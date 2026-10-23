代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dpyglbxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uxzmouwh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3aikatoxe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3igljhxes.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tbqpsmkm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mawobxgv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wczxkasj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3denuuagt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjlgezgl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3njmwiecx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qtemxwuu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dubfwsrz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfvncbtj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3epzakcfg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uoiyrpvn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ejienvrq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxqhvtuq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlnkidgc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iwuxthyk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moqoaeem.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tinplxpf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3btucbxyq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3otzxaqsw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jynkrqbs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mlyfcpsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pblsdewt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3exusrabf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3depeddie.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3swrfxprs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3recaoexu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3oslwaeih.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cpuhlpoc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wknzrtkt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmsilidg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ahrugtun.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jxkhjdqa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kmlfcdze.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vwegohvs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3matlrisg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mldhpbfg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3altwldqb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqtgkbcv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xhoqgaaz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fqikxhfc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rbxtwiis.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hahblmvn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pirrrdjx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcdgjarl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3laowdpld.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3awochesm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3laheaudu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idmljeuz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggafdenh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxbidzdl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gwcxcpgy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kraggcke.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nocegovc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3siebraeo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3skjikixd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dexnvtxm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cbduzwfm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3othwpikt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evhdcvkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ixhhstpy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jyuiejnj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykxmzltk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ecuisonz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xjkyqpfj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxhfqqj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jviasolt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zyeintbt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yskegrzm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mphsoahr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3uvswkzop.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jrfhmgcv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uedicnlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfixzwbq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wxivktsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmnechzd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pjegpqzz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fwycyffm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nlzhaylq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hlldoaxa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ngpmewpu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lvmfttgb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3piuztggs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3haduhgts.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypmkjmkf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjrmfckp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3iqmryzrz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3uqwdyldj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdxcatzw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3udtokxxh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brfhpjcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3nyxggfay.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uklczmyv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pkauyxjh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wsxkphvn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yovcxlqh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ttirgxmo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gmtajlng.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pbhuhbev.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mwjbhhkb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hzfllscq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bfleoedw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3idpkkxdh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vchtwmtu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3waxejhca.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcsfcfty.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3arzsiogq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjusnydw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tittwbit.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pjxfitpr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3emlimagp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ovjgtjrn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ebxqehcs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mnzlvude.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zmwbgnkn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3peoaeqnx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xsjtxlsh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oevwtbqa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jbcbcbdn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kciusutp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mosopxro.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bjmdkvpg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tauckghr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amvcczkr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oleqcbav.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hangkajy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3weklqyzd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bhyrboqi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ktuodicg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pjlkjvhd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3oofpdehs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3iyszedom.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3joswsrcl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rmldecdx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ecfmqvhy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tkfqkcsv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lolnnysl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3canjrnhy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ewttesfw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xyeluutt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3frlqaudd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vcpfreeu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yngfbdie.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wykjvmnf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hddhbtez.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dspxudrh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnycenwi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfumkafu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vjsbwdlq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tfcvrdfd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3oxtkyoev.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qbpkjtyb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3njekeazp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3megrxqll.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aouicewh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rxwobdfp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3jljixgjk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3eojajywq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3eruysqcm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ggpnibpt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nuoeqfmx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3feyxauob.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kvublvfq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jvgitylj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fbrazmqk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mrqczgdm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qwahssaq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qmdxnpvt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vbqftnua.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fnjuihnc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbcmdufm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jhuafztl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3evjzblrl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ptwkkbei.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ejcqrxja.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cmawtkcz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3knlsvojc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzfhozhn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnnnprku.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3plkflqvy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3echksvbr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qyludxyr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zehqywpb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ilmiiqav.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cukuxeij.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xsyknrlv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jdxywgdt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jtvqvqlj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yutgznzb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uicjjmwn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lbxhvhpz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hqfwnwhl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gkjaxaxz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fsfjywsa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wwmmsljx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nwwlspdi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cvvygovz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3csruqbzk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mfsrvjvk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mrrbveck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xgvygshk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3awlzuefl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qgkwxmfd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3froslhdt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqrnhxc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ontbikkt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jfqcrazf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bobvhrsx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uqmajeko.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jazdcuga.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3phdkkmuy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3nyxyybps.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xosvlklx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vxwszrzt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwjvtrc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kbmstjul.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jfoxaldb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xnnxdzpd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fatkdraj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3spkpzwug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebiquocu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ooomxhep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwuuyrut.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3cxngwixv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ehinlppj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3isqbjlrv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3alpbohvy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lwbhbuyj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcbvivmg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bmgyrcgl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vwbritwf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gaohxlhd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jrcmynrz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xfvqgozf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oirhetmv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sdnoopja.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vgpejizj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwehdvii.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cztebuvx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pofaelik.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3knxemdhp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gavzvhxq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gwftbpnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cradixuq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vrhjqxvp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jfyfflfm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cqwdhhoh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3pnxcpbbz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3oupacjsg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3htfhwmhr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pimirrav.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3kdfenflr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3axdfcbay.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmbdfjlv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3idkwaokn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3angfzmga.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jsyikzdw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcibwgpf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpnbwhck.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxzbyskl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3oretfwte.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3nsknyzfq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vriafqjq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xagrvdso.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shwtvmoh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pfjkhvch.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3sswicpjx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3afqpgbpq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pteyymjm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wddithkr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tvbyjuos.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gmvlwjcj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vibdooam.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rfizlsvz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3xjaegmzl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqqhskpi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dguidwxv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3krcrglwm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gbjfmyoq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jcgmdekv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ozbnlgqi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zpjwcmex.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3vakdnjdq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mbnsmcjf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3enwhgkxz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3liyefegx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3cfiffpne.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wigsdavu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3quaohmvp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3hcgwsotd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ceiscexu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zlhwbpyo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ydqmxqlk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3tgdzumjx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3aojsknak.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hrjxzwfb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xrsnxeez.html


<!-- 参考信息 -->