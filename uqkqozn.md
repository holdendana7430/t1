代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gvmsnzvqk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gasemdhhf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gkswtiqfj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/ghbqxxsbc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gvfrbrnyt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gcfnyvnph.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtbhqonfw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grpreegen.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkuqdnxcy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpabdxfxr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/goodxekze.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsxiyudws.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guavirinn.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gpsxjzkux.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqbojulfm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gijvgojcf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvsxnarxb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmvcozhwz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gyjxjwiqi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gezlyahcl.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gloliacfu.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/grknahukf.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gpehcljoy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxaqnscr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gmktpqcft.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gmakulcbo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gsxkwgaxk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gbhdrsbng.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gbsnrygdn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gkbpdmwom.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gstwmyykz.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/graqcfxxg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gxycrucjl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gjsdsvvba.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gbvvpyubd.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gzuitogmx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gjjdleldw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ggkplgoyo.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gnjqbdvcp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmaixnrwn.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/ghynkggqg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyfjoygzr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyroyixtr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdlzhcxai.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gduqidusw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gpknadrtb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gbknpgncq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkzfnxtxo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/goajlwzzp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gdqoclrwn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxapbfuel.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcbjdizdn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmjfmny.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gacedkchd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gvqodqgcy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giwzdcifv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdiqnqkhj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpanjqdsy.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gfjodfcmc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gpafgmlfc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqmrssgtr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gipbvjtxg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gohwaimva.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/goxbqlbri.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/guidlxjfu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gevvjqaxc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/glljkakud.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gcemysoxp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gqipypokf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gghbetsfw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gpwbusoew.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gxwynfwyh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gzzeulfkg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/ghjcvddoy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gsovwsjsw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gtuisohks.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjqnpzjtb.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gausxvdrx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gthmylcoo.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gtxcbmzmz.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gnevoprmu.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gvrpyphjb.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gqvxysryc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gskeuzmhi.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gxekgwqxj.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gvagaqvmf.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gpjwhjzlf.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gzezboncj.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gbmaqrqjh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gutwsouam.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gadnndmff.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvpfxndzu.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/glwblhdjh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpebfckbo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/goclkpkrq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gstblpucc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gzrinyvwd.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gmflpipxe.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gtgtsvpun.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gagjfspty.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/goqidptpa.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gdllxzbqp.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gwqwibqje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gjftovlky.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gzikbpvys.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gvdfqkwee.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gfefvhbrx.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gkfgawtzx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gclquublz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmftvajdg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gmgbhzppl.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gelkfqtmv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gpowyjnzy.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gesjbhxih.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gabuauefw.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gapqdgktk.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gfgaafagg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gvdtbrjhe.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtevsidbf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/giohqmzts.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gsbnucpkt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gwhkpmryc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gdahqpzdp.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gjaplbbif.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gcsmjhdli.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gzrhjtcub.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghpevrmnk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gudbprwin.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gdoeyhzmy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gygmwkyrg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gpamnvaof.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnrxqhqno.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gvihqtchq.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/grlulqsgb.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gmtlmzfid.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gbwxvbjeo.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gbjysxtoy.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gnnauyvzr.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gnaflzdge.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/grzjxcdtw.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/glwkhnsed.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gowaxpyxp.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gkvdmywab.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gdhxfuaap.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gsrvyxvlh.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gafebfwjn.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/guoutlryc.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gjvthkxkx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gmkvnglbp.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gjmejscaz.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gooowxafn.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gxdhzdgme.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gtqokmxza.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gqgucuidd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gvceahcwe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gldbkspnz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gtsmadnsr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gbkhgiscn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/ghywyixip.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gtbcipdkj.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gzqejcwvr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gdoviiaih.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxeixbuju.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gibpaiqzl.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gktetlokm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gflbmtnhp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gqzysuxgk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gjcdyaayf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gbzwiabgg.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/ggjalcttx.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/genlgzqob.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gipvixwda.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gwhbwktwc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gpaoujehl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gznnabqiv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gcnpogxfk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gzmvhcdqk.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gaamapoms.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gbubkuabl.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gyebojdhl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gtqdmnmkc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggvfqthva.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gtjgawdgf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gumhcistn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gjppfaxkz.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gurwtiidb.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gjmryyxwl.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gbpebbhez.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/ginfiqmoa.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gcdqgujjh.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gpzrfmyie.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/goecuksvr.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/ggxffagpb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gqpysgfps.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/ggpnvyhju.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/ggqykhmci.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gxcpckncv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/ghxdkskcz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/ggbkfkjke.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gfvvelpng.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/glreakmdr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gnrzufjki.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gtbcxrzto.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gspiijovk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gyaaetegx.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gdtacnufz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/ggjrtrcfc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gwenomupp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/ggjzeibvn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdvlepkrp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/guxwqberi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gvbuonmhd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gahlwowhr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqoebsjfd.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gvnukhqyo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/ggznpyjgs.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gscovplbv.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/givfdayfm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ggeaooimn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gcygtglza.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gysyugxgd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gvwtgqymg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gdsfoimja.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqrzeuimi.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gwexzmdti.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gukgencdf.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gbflhmgqq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/glutevude.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/grmwezosa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/guygmjkek.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gqkkdxgaa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/ggqcwlfvx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gedbpbcoj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/glgtallin.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gmvacvbfs.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gzcxixodb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gdluadxpa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtlavsicc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gipmshuyo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/giirzgcle.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjzmxmuzz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/ghomcpkcf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gigrmuouz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gcuklpknm.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/grhhzgmlp.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/ggcomaeqy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ganfpatwk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjrzgwvzd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gshcowlpo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvoqpoqet.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gjtjqskok.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/glhjjiabd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gmgsjrnzs.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gzbsskesn.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gyivieusj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gmhnptsxr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gcpuuhbhx.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/goxsovzjm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ghunkdvdg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gyrbkgenu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gxofkhmjx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gllbwpuva.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gozxvwgvi.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gvwfnsixp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gjpxybwae.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gzaejxkvq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gcfzythmu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggpbnhglj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/guhdqmnsc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gabbstdbi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gpcngpbtp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gkkaddnqq.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gpjockogz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gqbkdtcnm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gcemmtsti.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gfvxataoy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gllquaton.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gpkyzccrl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/ginsodoim.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gbbepfbmk.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gfcerwnjh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gcnrzlnmw.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gzzdjfgoq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gkvhfnrzg.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/goeccfdek.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gdcmbqiqb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gytqrzrav.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gmjodnnpy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gkxpnqusi.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gyxeaedkc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/giwttcpya.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gpgavpjex.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gkcmojbqn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gmcicrmte.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gjfwzsrgb.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gwqghltlw.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/goplhnbkl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/goktejaav.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/glljvgubn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/grylzbxjh.sHtML


<!-- 参考信息 -->