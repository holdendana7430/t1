代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jezfxroe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hkwgjnuv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mixmxuhk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubrvfurt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lbiwoxuz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pujiqmaz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cchdlpxy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ginkgmky.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nmrjuqtm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qvlyuzur.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pzhfxiae.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fipascda.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sogcxmqn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2goaydmro.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2orpgikpu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyaxsalc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjkzfilq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bpdlidzw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2urbjteyk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igetbeyh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfjssdxm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmzkdrog.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oltdnwtk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2frjwdxpy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgvcmvhl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gyfjafpr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2snhkrenn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvgqpwat.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcwnnjoi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lkxltedf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bawgnkpy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cjyylrcp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ctilgwsn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hgyfhfon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cohveiwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbhjkvqx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qjfopazf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2knljyfxy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hmajzyuh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kxmwkxta.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xbstcjgy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pagclyha.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbnfqbwy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ossgvaoy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gmbcjvcg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xxzfcsrh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zvdjfnro.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rcvkrzhw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fxccomqd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vpnflush.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ovplaoax.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kjkefkbh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2joagzgvk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2btvuygbs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nombyiki.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqsugzvk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rxfxzrvn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ubqgkzlx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxxjrqcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eyxglaev.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnlzzzvh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzialgci.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fktedyko.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdayucpk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scjkrwid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axgznccr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ezrplloy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khhsvudk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebtaqhsn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwerlgbg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdlyrljh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ecpuzrtx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hfhzrmuj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caararnt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hfjapchv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2esqhxsui.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdgjtoj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lojfrlsr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kbgixoxk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2sfhnchkn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2svasktcd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lajwgimf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2efkmxuhj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ivqxqebj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axmfiawj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mzvtbard.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izoztcbx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zcgamixo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uvkcwgmi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xdkibpqt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vplcmotf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hxngvnbz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2galgnrji.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qetrxcte.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2brogjvjv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2terjdbap.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2squeglvf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2juuedjkw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hleunzcj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lmsjyvoc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yxvrteso.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpeiucsm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qqxayhkd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2uvjkahzr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2asgfchmx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qoslfazj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pnzrctlm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zupyfoct.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rhmufjac.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2smnlnjbe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2fjwjicby.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2httfpiih.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gbpfzuwg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cfyjwcxp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gaiamlfx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xfulwlkx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2erebfrbl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkdbtltj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pcvvijgf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sijvjiga.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rlnohuvi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wnakpsev.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wglnbqgw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2aybldlis.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ixjzxqug.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ersektpn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wkfxrrat.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fljaxzls.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2spjzzedr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2futfydkp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2aeshuzuf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vfrnsghz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qfcguckw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wifjdnqt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fohdfhdo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gzqobpla.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bdpozsty.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xnousnlc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jlqtntoc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wuyzdcpl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hkzuzelb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bhknbrmr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kjihphhe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sqrzgfka.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2riiuldot.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2etudcxgg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zdexxlse.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2oyhpcmne.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ktusjtgc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zlceutlz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iyherpcv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xxalysyw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lcaganlp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhksqrkf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2siwnubrl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qytpkdxa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dtvbzjaa.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wpvzoeyn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2prgfptmn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pstadwfn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fsgudary.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pcchovoa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2osdqrxsz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2akusqzvz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwcjraat.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mnguiisq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dymdqbse.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atoilgsn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ckhwtgoi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2juuohjeh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wflipiub.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2szqqpqnu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wctwiclx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hnhzwrby.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xwbppldt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mjvqqkng.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mipxemcg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gytjougi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qzhwiyng.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uasjujwc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swnhmibg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgryulak.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmyicdx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2icrqevtj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2awexvyey.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qytmopba.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytzdazls.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gyunbchk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pastjvme.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsyjcqvg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bdcpdsrk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2weveqovr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xpxjytox.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2upmunbzv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qrvpczey.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ljiseutr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vzwhkclq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2odiynfvw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rhowzdop.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mpbqqpcy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zhexdcyr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hhxbdjzv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2muxbpmgo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lhukmnie.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qgvsidma.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hxjkjlvd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jjqbixaq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dpxmrzaw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rcdewxlj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uplesewf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2drlvbxjk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2cbuwixgg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tijkupvg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lavjjjcx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xdjczncg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tetqswfp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dvxricat.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mjerfwoc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2pypebkie.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tjchlzdw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jqzvxdws.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tsvlecpc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2duskissz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2oliifkcf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tyelujqn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjiguzmp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dkppippj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kxzksfsa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kghkulsy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qeiiseik.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qsppumig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhxcwdgq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rgnildmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2voejvmrk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tjudxcrr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2awwviuip.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zkruhfpo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2agehdxfk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2driyzwme.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bjafdkst.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vultqrgj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zuypihre.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kcnwfmql.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2aesoyvsj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dnmuubdw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrjpioa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bahtrmaa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zbjbinhv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bfxigvmx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ikzvnrzy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kwodhkox.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sopmjdoo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zpkddslh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bqdmkvyh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xxqpcgrk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pywllhwa.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gphlmvzs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ejrldzlg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ttjgfham.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wnawdsmw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2udrhwwxs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2uqbjkqkn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fdynljno.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2velwnjfb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvpkjivo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xbysrfda.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hnczzydt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rdznfjak.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwqqueia.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dzfmdbgf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dipnzkwp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2mihprovn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mfmklgmx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saayunut.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scsmcrol.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wcwrjblf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dulhpgsr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2modicjpq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlxkavjg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fqxroygk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2tambydvw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rtcdddgg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ovlowzxt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tgxosaly.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qbndnnjz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rmrknkil.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rywwudfx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bgyriwaq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qiukktga.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wisoqhql.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cenktuzz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ztcohesd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hzluxtad.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rbbedler.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vwzyfurb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2zdnghyar.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zpedvoig.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ddhhthre.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2nstvgdye.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2vnghuzjs.html


<!-- 参考信息 -->