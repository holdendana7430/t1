代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kkodbhlw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2uqunmbbn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2promcaym.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpektcom.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vfkhuoij.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nxqnhmwe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bbvhlmll.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wjvdongb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2agqfneyp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ruawgyob.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cgtjzoka.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uzuulwfx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zngkhwtx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ewvapzrn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xaqntimu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blhdlzdz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vatmqqzw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ecmcovoq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ammgvhmg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2maftegeq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wximvshp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gwczynze.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsafdoj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yrbhwqza.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcroozwz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esvswsfb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xqpreffr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbapyqus.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbcikenw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cosbzqqw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pirckndk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2brcmcjti.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ekhxwhbx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gqgmseeo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hhuxbauv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xovikyaa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhftcif.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ffigzerm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2tkpdcdsr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2sllxnhzr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wphnsmuj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mvrmetnb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cxmejzeb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mdywhtkz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nwlfcsnz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2djoqdkvd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tpgqvcma.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mmrznwhq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2azcafntn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sftakrfi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hnowexoa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mkktrpsq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dokizuzz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pnlixyeb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tklxeqtl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwseueid.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bzjwjpgn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2iserxrpj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjdkmujb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nexipary.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fosufjow.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvagtbad.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dantiigy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezocwign.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hobkteci.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nggietby.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jexknumw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfefpwmj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2duwubsms.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmagwsme.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvflofca.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwibmuia.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vwjibsir.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kidrjaar.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ogezjsab.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gmracwkh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2afttzsso.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bvfedlwg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lwijpths.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2erqamlqd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fqpvwhku.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zjygopzg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2iewjuqha.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rhpfjokx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iopjwfqu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xodtzrwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkhzlvpj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xzwbfdzg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uemwfjfe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpgyqlfo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sdpagtrp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jageksbw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2towoyqco.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gtnibssc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rxjjttrl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkwsfzpp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tlplpffm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ukawnpnp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qfytjfus.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xgtnzvto.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tlyawxff.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ltaqhfhn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2clxzqwgx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2filkufcj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvhiywdr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2thpwpidd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ddecsrxt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mhbkoghf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xjpqwklz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iuywudvj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dlvfqnsp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2znapbkfw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hokngdss.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2crytikfl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jesdnpnd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zddftzmq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pouzddbm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwbubtd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2frngwfee.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2firaqtcj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cgplxaei.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogipwnhq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fippuzob.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2cwtcbzle.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xaoglato.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2favdtfdq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fwfydjsy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bvgpnkuk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ikyicsli.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vmvuajkw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2drcedify.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2oxxpzugx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2stjeraca.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wumbobay.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jtzhctbr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wvhfqoub.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nallsvzm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yachdmoc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2knlkbxkk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2asylkjzl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dxvopzfj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nkrmeyje.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2iiimarii.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2reqconsb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2srnuqgwg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fyqqusrv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ctldhfdo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sdgxbwvx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yurpbdfp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nfjieqea.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hxprrtnr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ygownelw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkezzapz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lltwaioi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ekeqfnfp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntjfatvf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xykkktmm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ntskqjwi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dwdlloly.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2abhjxvdm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ngcoawuo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tddshvbf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cttxjrsu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2afutmwyz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cxgreetb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmbyxvip.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gojcbloh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gcznlzji.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ddbkxbwr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rmtndnga.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2neyyldap.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nqtraacc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fhkrkphw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2whqfiain.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ouganjyq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uviwyvtk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2picrjtpv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2udznubrb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2oedlgkgw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ktucmxsf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djaqzble.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wojmtjdk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fqqamlxt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jtynshkn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vozwfpfs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vbudxwkh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aputildd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ddiylgij.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wfynmfij.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qtswnxil.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jljvdraj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdkefako.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jpkoovlp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqmuwpag.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ibieumoa.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2easbgebn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hntkqvoj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fhsqivlf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ecpdvwjv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2inrzerka.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2adpnwccv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dmcalvxp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jqitkvmo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jwtykshr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2drysrlop.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ctfkflqg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lglwsqxd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iqdslwfq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2eypmkdku.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iawwrnsd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kyciougu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2efwmsftk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2clfhmymm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jhfhytdk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cplkxjgq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nvruexvv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dfnishne.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lkeojrzm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yffcrwcb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zldelpqn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iihjfbfn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2izpelcts.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xnpkdyfb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hemvzfts.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ujyoegeu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2baxxsyww.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vrxrjnei.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rocenkjz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ugdxhqas.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qdzxunip.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2iqqlfjpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kosogovu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pgxjoqvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibzrmqty.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wibiakbx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sjiogmgh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaribipg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jruammsx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2adxkpcnc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iojuvydw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2valzvrcm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2khrhhtsz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uiubobmj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2urbviixg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jpolyaal.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rniuocbq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kbmcqqtm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtszywvn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyokxigr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2tbibdosz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2utqxvicc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cnaeeehh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uxgfgvqw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2uxouijbp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rpezbmrr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ncczmhhn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lgxtjiao.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rhvxnsgt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jzehksip.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2etljjgwo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tnfoenrs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qpzaiqpu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vycaagbb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkratqne.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2iiictmhn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kastvpiu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2otftbrzj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xtiqdemn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vdbptjhi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxkiozhc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2itqccwtl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2svpaewcj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2giotlzlc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbtpfdss.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcvlmzif.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwlfhzmp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2yzwswyid.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2gxzioozx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkbhjzft.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2eiiwgvnk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2yqsmywux.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jmjbhqlw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fanwwlez.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qtfgtxro.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2niwllxjv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2msjvpydy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2aclznhkg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vcdyvqul.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2esfmsrrg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2khhawbmb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nlmxwuoe.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pvaysnft.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jxahjlkl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2yixhykzg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dwmwhayk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yzaahtxt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uydxmhxz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2brqjfwun.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pfywlyhw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2arphjxfz.html


<!-- 参考信息 -->