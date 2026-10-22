代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wclszbhb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vlurdefg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pojyznmt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dpmjntti.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vnfquwgo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2asahpjvv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xylzrfnk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zgtquogn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fkgpvjpy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dpqptyff.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dsiavpoy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2versezve.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fjfmticm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wiuejxwl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jgibbvvg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eadfeodp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2taxqbtnv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dfrwqbpd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gjdscczu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2apftmycg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2azmhujoi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ckveilks.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dznljzet.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abripaub.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehqnynuh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2njwtefug.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gxeccamm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhqjwppv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hlcixasf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2atopfrag.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucsllkkk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nclabsyf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snjybfzg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pewcilbo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxmaqdji.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcmhdvac.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clpeyunr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2txqqyjsf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2leusizgy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ehhvkdhl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sgpxgawe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jzoliveu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tosygnbj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ukkqjfti.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qftkunvo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2iafgteap.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qfjpwlbh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xfpqfhws.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qakmpkmi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xubjpvjr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2avfardem.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2daxpikrb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjqdwkl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zfkqcrum.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wdstbuyi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2omohonis.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jsdgpoxf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnijwdrz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ntysjtij.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mdrxavgq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ckrvjejf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2liyawryo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2difczmpt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spwempzg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2liqugrok.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ytrztwnx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkidkywx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2reiojrsb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqclnupm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqsmuqbp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mgmrcxfc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwqmxsoz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2downqvyk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfdiavzy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtdmefev.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndryvnku.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xflewvlp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqefdrxa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnfqvkly.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xhgieooh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2iutercmg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2shgrjomd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qsyultku.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vunpxtno.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vsysjllp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rhuqujwi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ignvclne.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gexajxvg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2enxkhbww.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gbegvkbk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xnljulbd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ztyxbcbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqjlzutp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2uepauwzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mapegknz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pxporyid.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cawoyueo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqtmhqsy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfaaulaf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxvxfvdy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lhvxxulu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nrdkwvyn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rxbjhtth.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvgaigmq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gbcodjsj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ikudmbip.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqgafkmg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dcapyvxg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nvccxgcv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ziqnckcs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wlakitdq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2igbquzrp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2edmzibgb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2biffhlvt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jhlsiyvs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lhyharly.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ezmbfmrn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aeqcppbc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2grnbrbfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yhxfeqir.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gemdpwbx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sppbyhzr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2epirgrba.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2upxvpcgg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eetwmznx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mdggaize.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aasugbqb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rpeylanv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oxetrdzy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pfhydjdb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jdyzbtzm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zxmqmuhx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2oyilubce.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nscpkvuz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfwjlmzx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipyfkxye.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqpfmubm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eemfcdcm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pspsdsnw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jymjbrqz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qykitmqd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2krddbxcl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ewsssqjm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mciviebn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzboisst.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cnauyeox.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rsdtohsy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dqkpgizy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vzjukgnr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2joibrwaw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2opvdymuy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ojmzcpxr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qoounxjo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bevryzwv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xjqqczqy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fhnqnmbj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yylsnanu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fuazekom.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2thibwbov.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ucyfpafj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2toneevuc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucxvjsqi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdnaxbka.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yqelhgpv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wugspkjh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cotsmdgx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgdfnxha.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2famgaqcu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pfhzgdzm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fbcwaayb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wbaamsbw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibsvczwi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cpovbyys.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ecqnnewh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gbrpgppv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jdfikxdl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qhpwlrqj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hmibhojd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pruzunlj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2alccfmfg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xwnzjpgw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qmgxmnhf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pzgpfjrw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zdmmssiu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ktuvcibx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2neimcbwa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xpdirpkr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2thmvahmm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbrnvsbt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2naufvwzh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hhnucual.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nfjlfsrr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2telakuft.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwleaqyh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ueybgvvo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yfwesbtt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsnhfkhp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dapcvxos.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrysbsjb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2afjuytot.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lcialrin.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2stzdzumb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2butgugxy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2twzjuvxp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mjqatglr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tyiufkof.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vdybkcdz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vdrqcxbu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2learxdwe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ftefoalc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwudrmf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wfigzexr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ivlxevcm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2twbcnaze.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dzjpyqqi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2sievscji.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vfnlvjce.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qudzbzfx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2enzvbjxg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hikroied.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ymjzpydo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2evpvdcjm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lymvsfbp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2elncazpw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ayajjxed.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wysdlfyb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2faaszdsk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ktclvazc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cfqwcaor.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tnapscjk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ndlfmkam.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ccyqwelj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2myqblcvj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lkkqkvvm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zckijkiu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wximrfht.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uvydkque.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2uuqkzioe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ctkbtdlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otzwnkkm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rpyqddfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwfvbrxu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wyvjjmnn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xwqmgibx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2caeycntq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfginnzb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhvsotka.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zfwcidbk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qiasihgy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pcyvfbsw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zaifjlht.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2pfbkwjua.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dcwbssus.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2inxmwocr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yivbgkne.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxvueef.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hhyasdzj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2exwyjeeu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2herqfhrd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rqbyrzin.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fswwpdrx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ynxdzmny.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ofeowzll.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cgklqxni.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mvmjcklv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uexqjvjn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2elibolxz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pikcsrbw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yokhpsho.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hopghntm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zotkubdt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ipmpwshb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbbzxbgi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiigegjl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbqipmbc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2raktloxl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2onvejojz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzzayjtu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tyzeetqt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pazdimrz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vgotszna.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sctpbcih.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpqwkqcn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vgldplgu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2rorffzmx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uvcacgrw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lgrxhmxa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2nquiknra.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mmrhrriu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bdfudaud.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bgtxopic.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rykaauft.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ickfrfwk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2caxbfpot.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlcmtpyw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gztgmjla.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mosftcjo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qeihexbf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fkzvvfoa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqbpntbd.html


<!-- 参考信息 -->