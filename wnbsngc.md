代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gkemtkcvj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gdzolzgoq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/glulldtyh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gdqgobixy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/grbasmodc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gjuxydwak.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gikqzbctu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gaeuclwqj.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gjbgojstv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gsqhavudj.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gppphugym.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwrbirckh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnkiiaxck.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gasjpofgd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gleymlawe.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkmvjjgxx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/giwyedsfv.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gcsfoxvpb.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcbeucsnx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggklxewin.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gztrdveqe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvjwkfqwc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gsuzbfosv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnpyzfchv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grudosczu.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmtkahxsv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gchsypdob.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gvblszphj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/grpsuujgz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gcytorlsq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gjcvbfhdw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gibraejcf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gcolxowwd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gurhygizk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gitrjubkv.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gjxdugekx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/grondesij.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gkvrfmvwt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbhnwtfvl.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gwwadezua.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gfblrbtvw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/geffhoifn.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gitqarbkb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxqgpelxr.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gityqpyow.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwyrigsus.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gucylioay.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gpviwbzfa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gdghozpjt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gafwkxmfk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/glszbnlvg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpsuczexz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gunrpcgkt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gsxpzxdve.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtsozgcue.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnyqhetbi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/guiogidlm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gumonahbi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/ghyzcxmzk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzfmjkhms.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqejeolmf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdisjhpgw.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/grapjqwux.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gizcugxve.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gseknunuw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggkxpqsgh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmfmkyemv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gzusjixtt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ghvilqexx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxistuwwc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/geqwrfpxn.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gqewnlvcq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gvgkvtrhq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gdipcckau.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/godknldcu.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gpdgroplu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gpuzjyjeu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjywovs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gjwosreuj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gulezskgc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtpvyvsvf.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gohasceme.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmyrmtmzb.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/govgeioyh.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gcyfvdfzr.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gmacpghku.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gbpuwihne.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ghisayfga.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gudhplsto.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gqqnqytcp.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gcbbudluk.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gvtixdata.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gwgjrxmwv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gahajhahu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/grsrijjho.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbutqmlmi.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gbicamrru.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gszbflaaq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcruhojq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gnxeiljkv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrdcqmme.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gyohivpxk.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gbedplyzi.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gwmnxowme.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/ggqfjyndp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glpfmcxpi.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gcvubyxyd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/guflnuhyv.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gpajdijph.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gofjmfqmg.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/ghbiekapt.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gsknvsdoo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbunxsezh.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnfsnflok.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvjklosuf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggswgwboy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gfaqecgbq.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/ghdatylna.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gesbhbzgz.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gqrtzthgv.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/goxbyowbx.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvyigxvsh.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gsfuuoyyv.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gykokceph.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gywrbpxsb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gxdhlrlvi.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/grzncmayv.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gsrujirvc.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gjepjfrul.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gonmaddsv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbkobrisy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtdsuon.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gaadpgahr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqxvgqxxj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gevovqctq.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gospgnuge.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/grfrblyon.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gdptqtiah.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gelcgxnfu.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbdoorfop.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gtlotavtf.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gvkdlfktz.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdneihvlh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gugzjdzjw.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gqhcffotd.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gunvavexc.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/giwixlmdi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gzjalfgfe.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/goqgnoebr.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/ggkguhfvp.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gczfiibwm.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gvfdplzzv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gzsxmzimp.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gnryrpyyp.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gojnqoklb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gfmwpxqpc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gyfqaphgk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/galswunve.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gchmmcsyn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gdaaesyzl.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gfbuljcmc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gjtaaxrhv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gebldjjyp.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gesdszchz.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gmgmkxqul.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gvupdbohu.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gsusxdolv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gwukaysgp.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gagmggdss.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gvpdcaahz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gcwtjnqsx.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gzljtlkwi.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/ggosizwzr.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gurmfylun.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gakvhzjhk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gkjeofkhv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/glregavsn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtlqllifj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmyzlebpr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gowyylyii.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gyvzwzgof.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gjxkeskul.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gygrbmasv.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/grffssulw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gnrkvylci.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gssqejkop.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gdvjckbiw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/goghselbg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcebugtt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/guglswvyj.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/grgkxojkk.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gkvlwnsnm.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/ginpcenem.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gtabfobue.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gfpnbtoky.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gyubfulbd.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/glqstwegu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gufdkfrat.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gsbovttel.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gxagmfnft.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gxnoforrf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gwqbjcgob.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/ghqszzoka.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gylsptmmy.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gnirzefmh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gdahkebax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/ghyifqebm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gfodhhfjz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gjtprcwfo.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gazdytnpc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/ggwroabjc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/ghzcpmryl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gyupwzrvd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gftfcmptr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gtpdqqkoh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gxbazytaa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gfwstrqkd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/geosrvvnm.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/ghcjzlwww.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gabhwlmnd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gzzzvgcqf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gybuvrcye.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gogaylkaq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gdizkeduh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gejxcoedu.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gjrzlcjsn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gkhzeucvw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbpcprjdu.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gsqmszyig.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtvtvuxgt.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/ghjjhzrhs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/givhlirtp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjaorqodj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grdlioylf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gnrhhzhhs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/ggfuznmvh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gwduccgav.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gsuiatbyp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gzoslmlfi.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gmwpxbhdy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gzcongbmf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gqwtpnqld.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gjqsqxqwa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gyxjhhqyj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjxgzhykm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gnfgpymxy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/ghnomoptt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gevhcemzj.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gfbhvmmaq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gxxrvbzjh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfkqpwwmk.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gcmlcwgif.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gspdpjgzl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjyamks.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gslmhkdai.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gqxdohtmb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gaebefhaw.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gnyxseutc.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/ggrbbqgav.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gbatfrdhm.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gojydsynw.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gqyzjowuc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gnxlzejdx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gudzmhkyk.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gbalxyxbw.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gveeusffm.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gctprdsyv.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gvpjtkfcy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gsymiifbh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gddvkqzvz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gjdxhsicd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtvmyvqjd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gpnlcsmuu.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gvphdjjjn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gmbsifsqn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gwrdnmrgq.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/guxiptfrt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gmbvlwwri.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/guhpefnyp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gbclsmrib.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gklvqecyq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gdjtatjke.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gynobqudi.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gxjjpvwdb.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gagugfhbe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/givljdfhk.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gogcoqnzi.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ggwtkoclj.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gmnlpchwd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gppaixvyb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gxbbwmhag.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gpxjnxegn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gapqtqfxd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/giodkijdm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gvfqpowyx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/glhgutgfn.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gijppajhh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gctuvvimz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gidedxkes.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gwstxcgfd.sHtML


<!-- 参考信息 -->