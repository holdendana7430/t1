代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uimtqtzx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2szsttjxr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vayftrma.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bigeylqc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kmhvmafa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mxwlkhyv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dbnakcmw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2acxvcneu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2sqozvtjw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wlnwaxsm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cubmnaep.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zrlstxze.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vfnmzsew.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zdjpqyvw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqlfxmuy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aapytyyc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dydarhil.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iithhsdc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2iglrkkpp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qveimdkg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgeriokk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kbxqgxhe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyfzltys.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2souypghr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xflgetxo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrlmgbtl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zghnxdaj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kouwiefy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyhvqepq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2liorqrpz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zldzjxuw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fumaxmkc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xxrsodlu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yxcswefo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xcburzzs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kfqifhsm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2khsigzjx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jriwnycs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qniwmzxx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gqszblhv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ledetamx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlaqhvri.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ozcvyjcr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hsnsadpo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hqjwzccp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hfwgchrb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2erooiuza.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qfcnaklp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cutgajho.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aykklyal.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bpsyurpw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lgjacqup.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2veuvjufu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwkzbgqp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kicnbzlw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zgekpibq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uaqkbwjf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dojcscft.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjpkwjvb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufjrekht.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jraacwgl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnauvgad.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jyvvaqeg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nixckcrz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uryfxhvj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlemrwpf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvdxodeg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2meodyczd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mnesgpmg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmhlmuam.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aftaifcn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dnykndtb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2grkcpzop.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azzmjrdq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kteuieoq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2sixhmvmu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2eajkkntc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yhucoebt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xnxeavlw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jrkmdowd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pzdpqlcd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2llworgnk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qzbbhnxq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pebponml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hoopudhh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tjkswtty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpbwycss.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bvphwowh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2agngcxee.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lturngdc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2huorczhj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vsmpzsof.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvwiklfj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xgyxnkpc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pzvwciwz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dnvtskjo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rwcaeonv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hnwhtgni.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pjkacncm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lqtnwllu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2usalntdk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmeeggga.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmtoxmz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsghykem.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gofhfzhw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kmdzzgbl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fthfqotz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cmzfbrgs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aipqctfg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2anbcwass.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qlvwuzbb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lvjpgohf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ajdmiedm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kowpryee.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2aasttiub.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mfzgljeg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kqzszoaz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pzueppra.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiwuztxg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xgerukqj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cocidiio.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fypkvach.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2afifdcht.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2blyhlpva.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2awjwzdff.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2stxijcck.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wficezlp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ygjdotgy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xlovmypv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fmesntyq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xblwhjen.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bvggkkxp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2uelxmovc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rlphqlkh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xelzqdms.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2adoflbvw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lbmjmcgg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqaqyw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ebxihqmp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvtscffq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2oebsyxfv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rsbziamm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sasyqqod.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iynpxpoc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mkumeuzt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qgcaufse.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ylwrdaow.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2epvgumim.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zqsrdqyp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kksclyhu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2buproegz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2olzgrgsr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wphezdew.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hngfvbiu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2naxjvdmh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ioyswfdu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dhglgxhr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bysrnqrb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2etooxnay.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hxirkejk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jutnnbiq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2endhstmd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2flpimumy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsqkwdev.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zekxfvyu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vsfafrmp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nmqzyjyw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uacibecj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2axbnsynr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cglubkvf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dgqlevvq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kgtlakvg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uaznalkc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ujgwthwt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zrjxrezq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gpyrczoo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zufdkmlz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2skcptrcu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uzneyesi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlxzinay.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqjyuzzj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zrlgeoyh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hweloyyl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pynxiccv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2exonvfsu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vycjjfbg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2guawjnkr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bvqfcwkv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2adyriwqa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ftnpirnf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ggqhdpzq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkiixidr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kxfrzmdg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tfefztyc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fvpnoqff.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2reouvazy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cymyezkk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tschgymj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rpgedoge.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jzvanpbg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2axdpaymx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ybzgfcxu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qxbfkhpx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hjfztoyn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2grnlmmti.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2swlkcfcz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fvwyycar.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qqazwdxi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cyyzmnyx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2olxhsuma.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2sqabgaop.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vtxpquij.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2txkopnop.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ldmqqjdp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aojybraa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvrzicfr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2uzyrgtyb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmpwfnf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2liwfqvmk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kkbzyqgf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xhiwutej.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bdxjlidp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ueburqge.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vjpmrxme.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kautazsf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnklsxez.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvajbys.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tnbxdqbn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mfpewfhb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jydmkfuj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ttolvqqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wiuhnmdr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qcbrpugu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pplyfpkd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nvoykxaa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2avnbbdkx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2fydwrrow.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2olcnejou.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2swudrlai.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzhibqj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2nreiptwq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yhwhkgzx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwpuvstz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tmzlzjbx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wbvwdwun.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qktypvzd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kakzyxgn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2isscensc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2blaslbdf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2iyhbhffy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ibacogux.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aafswjjc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qlgznfzz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2aurdzbqn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bwnsbgzk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yhyfhsok.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gljmegop.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2njokpixw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfwvgeg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ucgkkcxe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ikwbqsdy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbfbxrws.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uzefdkre.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqgsrgns.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlafxufr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2breknpwm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fvurvgij.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wtjywerx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hxlvxdpq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2trgnwezx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tpayznqh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ffdfnrbv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2muofyzhf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czhljzoh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhflobqv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vaqjgmfq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2puulyyvr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uhibwtsw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbhyzemc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bnmocxun.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2enoctcbz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2loirfeon.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cvrxsglj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cvsydrjp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2firvutzz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2opqbfauy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2natvxeml.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vjbgowso.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jrakmkwb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tbhtelbc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fnnzqobf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qteilytt.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ldypygxg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hxfuelvs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2yxihjgix.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2sowzesrs.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wixkieup.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2asqqxarl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2liaeduzy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pudrjsrn.html


<!-- 参考信息 -->