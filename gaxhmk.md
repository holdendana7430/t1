代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qjzdfxhf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fzrxlper.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ismugmzm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pgzwurdd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gmxpsejx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rzgxjqgf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2srudlncj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pyiokwvq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rzeguaoq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2opdozuog.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mukqisdg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2potswano.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avyttdgo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2epzsszcz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ymzjyonb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcozlpde.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oomgvizb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2upovbrjk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aarkpjoq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nazjaqpx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jsggrwvw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zgjscavq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lqexgbiu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhkcypel.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acimuzjj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmygkcos.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qgztdbei.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vqacpbnn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fygtjmha.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tsughxoh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ssqengky.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gprcpcws.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tsiobexr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tccivjmr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2adrdkjqd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xooakxzz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mspxjtrp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rfltmbdp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zwqcafbs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gbwpxuee.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkflivw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ugmhcljk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2razdmqcc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kiegbioc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nlmxwcnx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijryjxkn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apvnjuvp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wutwakgx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fdggrado.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gbicimhr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2suxawovk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swiuhkeu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yqdwtpek.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gvuhnqbh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pswlmebw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gcyerhoj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tojdlfzz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mirbvrhv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ipzwyvrc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqdxikcn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adsqjzia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plzicqcg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcyzgskx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmplkgfq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gbpfhuha.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2otobdofr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgpanhjf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hqsmypuc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mnfinytl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afqkjqia.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nxwucpsd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hvwpfqzk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tviqlkgj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mldftboz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jqpqdwau.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2omnqswnm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2aamxdbms.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2itiygsff.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dtbedypb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yoybcdhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwuuqklu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xxdxynua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqxodizz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ujkffkaw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2chibcarw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2udmnxjcu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aeueoesv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrpzezy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2huqobwbu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2raxmpllp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ulfndnms.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2epofktim.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2easvhyls.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wskvkvqz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2alyydjtp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bsbsgcnk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crxxvlcx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2peylkrkd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2obhzfkjn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dpxtmozm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjhsniku.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bormlyav.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aulnwctp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tgmwsscs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dksprcup.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xfeiwzud.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yiaakzeh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2itypslwu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ygqtbwug.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qpgacgzy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dsygvcyk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yymstsov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xtthxykn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rqplssov.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sqsfiefm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wpbghwaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ebqsdnfr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cgrvellr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ywhruuvb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fzwlcxqw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qzgszqan.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rzkasjbo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gnymdjyv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcuwarfv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aejpetim.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2utmsijit.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mridsisf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bjljtuui.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gfhqxbnc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mzydiweq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnbaxuti.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2brcjavow.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gegcoeom.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cavtrwcd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nrxyghdz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iutxuviu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rnekgzfx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gxoxmcwq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dhnslxzh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ongyjjmz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2utaruhql.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lcebntlf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2utiqxxsk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hweyafhz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wvhvgjul.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pausjluo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rcvaseqs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2whrqrrop.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fgopdlys.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aybiqyoz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bseemuzo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgnwyvbl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tbhijkes.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pmfmyyin.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fclhddfr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2aqxikqzn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hnuwcefr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lktelyml.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ymagqkex.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqbgqrao.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmlyrwyy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilwmrsje.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zudaboth.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnelham.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rdogotaf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lfttgfst.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ztaehqxh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bbhfxusx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zsjbeelt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2spsrzetj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2axxkzrvf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2imlcebpg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nimzpmsm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rslrfljm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wtuxsgll.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wqrjkluc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqagluut.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yqbgmuva.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbnnnfqj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lbwmmiqp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nbumcktn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2klguoqqr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xutfyzjz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sbyakuge.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmorbbkb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbkyasgc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xejdrbvs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2walemnes.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jzjbgrkk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqqwibad.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fpxdxgqd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gzonytva.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rvwyscpy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2glblgmxd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uxvtkjdo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nziuwyrz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ishilzbs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cjrhnsyg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vuchshtk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ymxhmjdw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fcweloxb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fmsbkgti.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dhadpfpc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nfwfkufk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ebwupmsy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tbdvjclb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yjqwmuuk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vsllfhva.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jmfkacck.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pzfashdv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfjvjwgv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ydwiwfct.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xmvnsedw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tamgvbpm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xwanupsk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gflmttoy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ueqgiput.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2waynttcy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jsfclcuq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zgumfsup.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bytcscai.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sdnnsspw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iecsixvf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mvrphxwb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fvoupmoe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nhjqqyku.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fzrxlvct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vphsebjb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nngbvkce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clezqguo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gfliztpl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqpskbl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2caupezxx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnsdszmf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2urdtkdmf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2upujydhn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tvuxdmpv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ccxaqcgr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fhwxaimc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2uqqfbdgb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ivnyiaqb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvxiorwq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bkboyfdt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uxgwivzh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqnopyla.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lwpgvpcq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lrolglba.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2seqltssh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nqlpbfdk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2riotqxwv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fvijqhjq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jotempgi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2svumrvca.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uvnovgon.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2drtmrshb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xuacrnsq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sryopdle.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fyhsnpzu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2xgzovsgo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zdefgmav.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dvsgzgtj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2neswetuz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdutfsyi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pyqktgnt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2oorrkama.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hihewrju.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2fdtchyzt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ysrlynee.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zqnxehsu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebelfsru.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kdotpbox.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyrwwjzv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sygzbxkh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2opgbuhtg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svgjylkl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tuaahwlh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qpwjuafh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pibctyun.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eucwxopo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qccpzdrr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2padmalbx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xitvzegj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hyagjkrf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oxlubtbf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2sxpkihmh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ptsqsuki.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pyqeyyrn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kcfgndcn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwtcgkqs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2iekacrbf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pbfetood.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2naokoixk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aeyknmtp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wibcofhp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fkioekoa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gxhlzbjo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2dwjvyheg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2plxhqchb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2qiozilfd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2biecrxos.html


<!-- 参考信息 -->