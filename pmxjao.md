代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zsvooxlx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ouhexhfe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hslsloos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kxihfsjo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jaobwoyz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yrfgjfrw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hsfshzql.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iofdmyar.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ahjqnorx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ylbjdnyd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zvpztuhg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mikhxlbt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtwkggqy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aaezhgxo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3oogldevh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjaevsow.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnyofdrc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3psmfpdtb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxhqryti.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xzzjplsa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhwssvta.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ertwccjg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pifrqjuz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smacxhil.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcufhkxz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zinxnoni.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cxtgqyuo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ayjettfn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ypptancq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aqxfkflx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kedbiwou.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmxnzpkf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3phwpvivy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rbcxihgh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gbhlqicg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ueygcqsf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vcibtwsf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbfjxdxc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ahdihboy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oezgvqda.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xcoeypfz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pzxggjdo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wucdysvh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3klwbmkll.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vlsbjjhw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqtjzmdz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pidiqotk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ndyeedvx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hcfhfrln.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3npucnmsg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vgyttxgj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zjzvfbus.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wyuwgaks.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3utcfxode.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrlkgohi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxamotex.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkaxrchu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dezennbd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cwgmovho.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3edstduhi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dimbkwxa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjuhpjoy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qzufafwa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3suretgdo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbnteyvk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgecyqum.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wznyuouz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjrbynl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vhkftqrq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3swtwrsux.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nnbesxpe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tvypvkut.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lxjfbelk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3enhnjrsj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nefcaroa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pcwyuzsx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xgchapic.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rvvalotc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tmezgoot.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rskxhdct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzyjauts.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zecasvxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlxwdmco.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3egfeewuk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3khpehycg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjjpafne.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qljnwlhb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bjmqtwsv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ynhvmgfm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xtkblnen.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yjadzkbh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzpjtifc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nouznpok.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pgioklcd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rwgqdynl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izpjnbqu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcixiwqn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdbllctj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wsjxnewz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfldiydt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3shleatxt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zyndtthw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gofgbigg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tpmkrcde.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3glhwomda.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hvyasqvf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fdmwejwm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vjcqsrkm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nfypvdqj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rtynrnex.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ymscxwgb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xliypucs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3txemplgl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnhrxzzj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usghiniu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ahzqpwao.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nomnyhnx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rbgdivlx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3inlmyrfe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uazrasbq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3aqhrpvbu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyapnbyv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rdwzqbtn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dvpnewuk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3olunrveg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qzmldneg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iilchihk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vddyzgjg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wcbrekgv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tyazxetg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xpovhgiw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywonjdsu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntspfbuc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3akfsqhqb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ssgasrln.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3grnrznbs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cfqirrjc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xcmjqwvx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bkdahuqr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rongkftb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lbxfnknh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bxzqfsdz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lbbwktiw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3teixyqce.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dkdwryks.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bwpfckoi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jxhsnnqv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gamymjaj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxgtzzzu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hvuzlztb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3txhtzpbi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3edowbint.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vvxmyayf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3floxlwty.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvcmsarb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lpnlskvn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ekjtrior.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jrfotapi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kqsmwyab.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gyzputhu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3yxveassc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3evgmelgn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dxmjggki.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqmnxvun.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ggbopaci.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3brergtje.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yyojjneo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vcmgupst.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dsrstxjz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3oyakggip.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kopjspdc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mlcsvgve.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nlwxxffn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3dbzzwaqv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cesnlbiy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rdzjpqes.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwbhgzex.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ectbnkjp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ebmxydwk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtqsajh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ajvssurk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wpccpext.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ztrmnsnh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kqzlzmui.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgzordag.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfimzaxm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oawyjifx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvunqxcw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jpdvfcxo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ntbthdzi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sipgakad.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dnhxutqd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dewetgwo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3llshciml.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pqozkldt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fkfnuzsa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kuhrekuf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3podghvvi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yunhmwuy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mqfkcywm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cnngumas.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3lrtsxcng.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yuzybwlt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fdvejivr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3guvwgxdo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xltmznyj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3nywxcpos.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dithxjfv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mmxwpyyn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dyrnezbc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjcqiqqc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3uiyccuhq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qutrjtxg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xjqainjc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3viknkrqn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ysjtcdpf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ijewiwzh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xntptxem.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rvfyzfxk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lbnkkqgt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3iixvjqyk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fijvhiro.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qlmrpbfe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3aiobqzoh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ymlyrtbm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3msnxfwyt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rvnthmzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcfmxmfz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3geqyyhdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kebgtpoh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wufhxfwq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mjgvhmpa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmqmdiue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxqkoux.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mjdftird.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3acjauswq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lqbqvigh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3nonzncbm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3yhdwbnxj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3pifhldcc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rrmmfomq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhfivchn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3anwjihqu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3isidlyih.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlhnoggz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3udxqumcp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsdcnein.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcudfnra.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3orptnwjk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vonmkzsk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ampaojim.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vpctbvjl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3afrylanr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xbuptusq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkhfbed.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ahbhrsvk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rshuhfdm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tgvwujog.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ytdwcgus.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wtnjscqf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qzopiwcb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vmerxnlu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ocgpisoz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3egzmfqvz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3qtdstmyo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkwqucod.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ybbarxsz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gzmlxacd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kowbpgbz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3eudduuwi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nhvmzejv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlvgdtjd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rasvmfpv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nqiiehwv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiwexyqh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pxkndobs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3uqvpduie.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ilfwzmvx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ckflmwrw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wflplbzz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3snjzhrid.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ipqthwge.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cswxigxa.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3fvgxjuky.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3okzeydvv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ottdhuya.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ilrsrfdm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aiqopykk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bmtjfvab.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gqhrefkx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ykxmqddq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3taxfclrn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xqsyrdlf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3dpolasop.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cbekczri.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3cgzymwpl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ujeismtl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ezprizcr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mshpjkmv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3cqytzjmu.html


<!-- 参考信息 -->