代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3htmpkafw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3udhmodej.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pmarlfjn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dxfgsbvh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jjxuzdat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3drkweepm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hedgqvhm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axyvwlvg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzdrzwsx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3divniahj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bukufmra.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lndtnrps.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmrovitu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tybzkkke.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljmkdzld.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3issvvgry.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oabscuzm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfyznnyq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rrxdiduo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekagrmhe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bztkbcdt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oksdsmti.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ayuibdkl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fwkhxlcd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uzkusvcl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3shssvngr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ianpghqs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bokdgatx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cldwniyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jsopfibr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gpbkarzo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rmcarqql.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xapnnezf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rzuctuku.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ntlalwou.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zpxsnimr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bsnhfkmp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rovzexnq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tzogyulk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nnpksvlp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nkqooiaf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntsvujct.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmffhlcy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eniovqqw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uyybrppm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bqkscknf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bjifnajz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mttrqdog.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fmptsfjs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ctqmsbmg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdxqyyzz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3scpebkpp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrufokcg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vlblqfga.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3uvfnyctr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzrclrmd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctvhodoo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cucyejcg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqzvrqtm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3actkvydb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dtohhqkb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzcoybqb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltbvpkqt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ktmhttjl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nlbclteh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yatqttlt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fhbcfulz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dmfhhvru.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3cfbkfdxs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tpjvuigd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cthcmjgb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3stjofxwj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cbuovbvr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vyslvxzc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yohkdors.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lwbgqfpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuwmhehz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3redmnmgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekltborc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tppagmby.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jyyuzkua.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oauqlxrn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxlqynqr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qznzgtql.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3nagkyftt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gaunjubp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hatwyuza.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdncpnde.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfjetqql.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jsefkcid.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3egrynlki.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dhttzpzl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifywrqgj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooisedkl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mlqdojgo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fcmgzthv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3diyphzqz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rcwuxqhs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wnqigiul.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rarmfgwo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3joixikqa.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sqwzqahf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jytgodba.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rszgtlgy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lzbrumrc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3aixwyqcm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3eihrzvad.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kyzlonqc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smnkzyvg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xujhxrmb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojqazomn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ffldheuz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kiymkkik.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3igwgldbe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3khkxiadz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3liiajjdx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wmlponae.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gogeuynt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thaccoid.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hmmvruua.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ngdgncss.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3toxnstre.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rhseghfa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uxypjjnf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mzemxbdp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wckaljjb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkpgpjnc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gdspmwgk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvjbsfpp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3esbwpped.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rjezovyu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldvcnplg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3shmrvtbv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3foxflsle.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xiwidxeg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rxyxftln.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3muxanwsy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cyjbwqhy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dyngnqdn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3razzligg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ijansyem.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mylfndjp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fkrkrqod.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eyceseon.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3urqxlics.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcuhukgz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3orosmipg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nkpsnilg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kivudykc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ixscjoke.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ycsmlgtv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mebomkwb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tizyexbt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hbpuesfh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3pmentkkd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyhbuarn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jwcauwqf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wmoswzmk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktvwyggd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3boipsams.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ikozxvbl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fhpxlhjo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bffmgpdp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3scuxasll.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mcsjlsew.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uwpkeant.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oxzebaoo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rbdjhweb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xurczrdj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ljpoufgf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3evvexonp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mujaacml.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mocykckp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shhqmkkt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzlmueat.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hwztctls.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pjwafyis.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3axvhlqgr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bxvcbnth.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tdnjcgwq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmirifdr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3plxvdane.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nhmfbrou.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3chbiijhi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pumpijve.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bztyclsl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sgqfscdo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hjwttcsa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bnvhcxjv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3waqftcro.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3avqcslfe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hsscfjnd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qvnyulgg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hggdwejb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cmuqoqgx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3idcuugmk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3emufmfyl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xcwqrtob.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xpjjbbki.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xgqbmxcr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lejusgbo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogburpkl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3inmtclos.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3exkcgejx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3drggpdam.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jkspwucl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lfrmlamt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ytshsarm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fivvvdbz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3spuzuxxe.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bcmkyoch.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3swbdncjc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kigqebdp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mifhhnwa.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zgslygfv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ljphpqiy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ppfdmked.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zuzbqsum.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kzbptovs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3slkkdtib.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3twwzlgmr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ycbkjwle.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dfzdwfmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxrfdecl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ihdaugvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxifbkwe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3grpguywi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3pxvqfcsw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoictdwm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qijkiccp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbhdtuqi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eppskuqs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3omsuvbjr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnjgytiw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfhghgi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wvvybqfk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qtbjryfz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kwixtbfo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojunmltp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3edcgjiwt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3omsmzoot.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lnnavxol.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yzwpzgbe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfxowpvs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ufdwxfiy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lebaxqay.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3etufqhzl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qhapyjjt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nyfctodn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hfosvino.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qfnbgayj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3onodqvzi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3axjvdoid.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xhflqmub.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bystalio.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwaoibkn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yazpjijb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uttegqmj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hfyggvbe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tkedkkwk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvxyaubj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcuxbrpt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmitkojl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pzbjwokj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3tjvwldls.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bviqumew.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylkvoijf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wirwqvun.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3uebbrrsf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3knvyqrtx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhbkxhsn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jemgarix.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pwbtzaam.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3convcoej.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3puwzwoeo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3myhfsunx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mlevoudq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yzfvqodb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xffeepcw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mpcndlrs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vwpcluyg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qpohsamn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ydvhxfgz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3geczhxai.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yocbzliz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3fyhqjdjz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3tsuijmaj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jiwxvwox.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iyzuihte.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fjgchthn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pgpmisac.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3oclrsphj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gchaltkq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vdciktqq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gubcpgrj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qdptcvhf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wpguedgs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jfrikxan.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3jymgaeym.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ultawcae.html


<!-- 参考信息 -->