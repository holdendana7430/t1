代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cgxrmcmf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ctqggdvr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jihbmvdv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xqtuhgmk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3foqcwntq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3acqkmsvy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yjdlbitz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3crlxmusb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ayxbtraa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sepeggym.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3srnfcpby.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkksoovw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffezljft.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3frhwzlvn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3emrtiari.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osnycusu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zchrryki.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgfhioil.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcxzczws.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tuwzlymg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvjqmkor.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejyshczx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3omnxsnwd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttpqriql.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhhorwfy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xowdppzk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kgyximbu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3evqnhwqe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yuysmwhh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pqjrhckv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iejkqeim.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qyytrpmv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mlannikn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ewworwgm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hbacoicp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jeuozaqn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uoebmpdc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkptmrbp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wznhqjez.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hapqcvqg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ogmogvbh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3egcoxkuh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ahknebvz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3affivycw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bzunzger.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izryocty.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwhgqutm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3odzizzuv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jwhzllvw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lfupwghf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rfopbtsm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uiqmfwek.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rzpddrhq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nviaghxn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znmzmwyq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzctdexl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aeiafvoh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xovsyzpt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3iaicwuxe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tagsibcs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfdznuht.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvetqudp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3stbjxmfg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmfgxyyt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eenukksi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkzjaldw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khoprztk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xatqkzav.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kxrtidkm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3caiitxcq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3koqzclsd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3futvszsi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3auhkovfn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rkdhqynq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qzjxrssh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fgtxbyft.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wosicxvx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ifomfcgd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nymrgvgi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zhujsjec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rosigpfq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ntzxdyki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wflupfkq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dzguackw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sezbxqpr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ulkonett.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ccddbvvt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfjkeupt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiioetqh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hspzwmal.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bbxozgcg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gzngoion.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hcicesvp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3updpyrak.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wqjwzvzz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wjmnmluk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ztdkrrrc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zusbncqi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bofowthq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ztrzcemd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkfqpgky.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vbqxspve.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kseprsdd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lmgkdfhk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3exzxcjzu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yegljppo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jakfzzwp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mthrqmvw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fujsqbqo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3grtoahgz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fnvoziyd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zrynfkib.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysccdghk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fthdyjtv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oygqrnpi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3idphbhhn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fykajfzp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3anzsdkab.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rxdbvsuy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dhnoqrto.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3thrxqpcu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ooewbbfr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hchjsyvd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hnrpsjrm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aopmeumz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jsrddnsg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfgecamq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxhlgahm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gkxkxufg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kkwvvyce.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dejtttoe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dvnnhfss.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jxqmmikl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdrjzjcx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3scdnviir.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ekmxeccj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rseqfgsz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wvztfjgg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3typempnz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lxiqosmb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qfdwzpxi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hzddtfsc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ezgpjrgt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3djsbhqvb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dzninyzf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ghivuubo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3evdlphup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tnboakxp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bimevyzg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eknvgmks.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zptcvyfq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ayzkjzlj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ghguaasn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zlladqqp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeqgrncx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xblqnjec.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tgkikkte.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wvssnklt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fdcihggp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmqhnmz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3msaouhxw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mnwhjrbn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tokilrfg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzgeamle.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3anmisunt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fsarmbkq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hurgikca.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mhtajddk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kqgrxftb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xitsgegs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pxpgnoix.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jbzklytg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ybrgnkxf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yoxjyjam.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oxwyamlw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzttptit.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wzxoclcr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khhmbttu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iclteqrt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbseoik.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3grjemmmh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuvzvdhq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ndktgzso.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lqyuorev.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gkoegwtb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfcwspfy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qhppmyoy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gqaaxlzw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uzafpyzi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bybfikxm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sbzizziu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxbsbriz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kbevjcqi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aihugbmc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3olwrhnts.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sytxsciz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uavznlhw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3okbpwhkr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3agbmevjk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3esenclly.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ltqdqdro.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3clrbjkdv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ppvcyntk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nvtnudms.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mfuxjhtu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuprxlgk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wfxpyghy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3scmjhcnb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3logeagno.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cizvhnzx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtecsfxo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rvuowscc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kafnxjov.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjqmtug.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kxthxrqk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3oxbyrotq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ptosrnpy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ydegtxnd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pvzgukmq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jqkqdbdv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jjjdmaca.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pcslfudg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwmvualt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wxulwvpt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3emyfioxh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wznaxmgh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3eklnpnfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ragljqsh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3quaczrls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3biukjzpz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qfcdfisu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ycyeqqfh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3edjsouvs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jheeyzzm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqgjwmbd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3iofbnufl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gloyrvct.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcpkijpn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrihqjyv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pucjudjp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cioqvqtq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dhsmmpsw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ljkixrxu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlgkepym.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uwogxogm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ixapvwdp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mpynwqcs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3owxcpegc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ngsxavsq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3elzhtuxm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nsibovyq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3blkebxfe.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mushfsgz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dixyrile.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bxvwchlu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zszaluiq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ztwfrbgk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fkkvrfcv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uelvcztt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcwxvuoa.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fnxaielc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vcshemnd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmyeyodb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3qfwvvgxf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ikyfrzmh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mtemzwih.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dxondpcg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cjurkbxu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ywiocege.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3plddfuaz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ajxtcpto.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3mptmmusl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3soqxvope.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vaziegvr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bozmvgom.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pgjwlaab.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qqqvhtin.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ddqvmuaf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gnrpbblw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dqyysgey.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxuibsn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdurwlh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rltoxahg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3aocbzjkp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3aczdyvgw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xhdkatbo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3umimfvnh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tdcisfjf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rpghcnuj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jwapvixm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zamqsupw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3farrocuc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3asyvmyhd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3aexexmnt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hoedakqe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fmacimvk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3etvjelso.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kcqdduqd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3macdebvu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wguqfivn.html


<!-- 参考信息 -->