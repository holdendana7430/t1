代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gicgvnooq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/grcuyszbh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gmgejanja.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gitnggnsa.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/ghsjnxaqf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gmzvzkoab.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbkwlzndw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsbhrwdoq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/giedlfqzy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gvopvrufl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gvlckunqb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyzsaddej.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghxqqxsse.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/guihghktg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glixbltrs.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdxusnohg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqnsldywj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gorkphjnj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gpqqnyecp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gejwxscju.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfbcpwzrb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwckdmdid.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gzjxqzuem.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gsskzhpxk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gfyoyrrzh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/ghphyepwl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/govkacwqk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gweelwnws.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/glhvvqtcw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gydizrmel.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/guprtivsy.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gcmshjfyh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gsibpveie.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/glkpmdpag.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/grzvnxaid.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gmlkpqaas.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gqbuklumc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gqstjnhhf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/grlojlbiy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gbowcivqs.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/ghgegmrzh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfpnxwdgh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/guescfypo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gpoczqgfn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gpadvlywu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gbdftirkc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gmdteddrq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnnkhtnuh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gabhnvqwf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gjfgqnkfi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdznodmyx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gebradpjt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/glvkkrdfy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsdxlsxnp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/glfoyravt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guvvuzdyn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqlqqzvoq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gikrgwxzf.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gnnnexcqk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsevfbcge.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gtymxyxgp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gvhiipdno.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gatqbvtzm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gikanjowg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/grfcbdlmv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmpbdwehi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gkgdtimjg.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/ghxctrmtc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/ggipzvlcv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gohxxqifw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gbjafjjzw.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gbgwjopru.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gagjbkahf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gmnadguvw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gxwvsybmf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gnwcryxrr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfltmjpqm.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gawljaerf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwuadijpv.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gzdqkgpyl.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gsblrfqbu.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gtgcljvjp.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gvhxpvbly.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gzticquis.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gavavluto.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gemzbgqpd.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gcfuyuigw.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gdqglpzqv.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gjbkyanvx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/grtzvhseb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gecspzzug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gpdroxqry.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gclpprwva.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/giqsshupk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/guhkufyqi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gcowyxiqa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gghlvynou.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gtqrawpbf.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gqdxwncnm.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gjpetkohy.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gullhlscc.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gzfmgdpsd.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gprlxprhg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gskxulzht.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gpiakkuqd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gcdduhaem.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gctsjabsc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gxzwnttpk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpjjuhwsz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gnwdopkba.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbkidavln.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggsundqvd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggwmislyv.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gpevvlcok.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gmyxmqiku.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gacfcwysg.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gglddbfvu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/glfikudtq.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcbvjlbvo.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzacextgi.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcykpgphs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gupysvxpj.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/ggvzmfvxw.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gxhkjzoni.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gtajbcqfb.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gigfyncuh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghiebyoug.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gnpghypgo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbothgzst.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/glgjherfg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gpczgcasx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ggwozbpku.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gshgadgiq.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/githkrruo.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gquueumam.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/glukiekfc.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gdaytbtaf.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gocenovti.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/glhddjrvp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gpiqqmozt.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gmcbazrxo.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpjlfznrz.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gbkixkdah.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/glsvcmrki.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gvbwyuaya.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghlnwfgbx.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gbvyhofyu.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gxjqbuxfn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gnxkpjkvm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghldaxprq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbbbucjhc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gwmdzdyqi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gaggbzubs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gwruelxzl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gnuixoqfa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gyrkwzgas.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gulhaacvj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gujjgordm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gimbckvpo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzsdvavoa.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gyauuhsyw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gzsrghxeo.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ghmgeyjtz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gdgvqjfjr.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gkyuizyen.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gnjhnxuwl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gryzpylwo.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gfkfyjnpc.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/ghyptfiom.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gzpwkivlf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/grxbnquji.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gurmczzuf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gwhgfmllh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gjxstmyht.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnlbkhspp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gqmaqacte.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gkmgblsug.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/ghjmhnsfr.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gwojwnyja.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gjawmxuez.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvihigqnl.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gedjvoaml.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gffktnqpr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqsphfocw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gkrvycydw.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gpbcifupg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gjmarmmdo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gwyyoxzst.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gynysnzyr.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/giezrpite.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gqnvrgaba.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsvpqcsyx.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gcpxchqgb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gvvzamsff.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gtxdworai.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/grkbeqfwg.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gyhfkfyft.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gqjurncvp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gxfpsqcwk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gdcrqhfix.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gkfqlukxs.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gawnlgsff.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gquqmbxtm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gbjyvicyr.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gitwnkndu.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gccjyvxip.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gtjbxymwd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gxyuqzaxx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gpgmfjdwx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gpqahnciy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gtksghdla.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gorrozyen.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/ghkwdozsx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gxryxpvbk.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gpxisqkld.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gfofsiszv.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/glulzktvl.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghabnqyav.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbldmcqjb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gymmmzidz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gfbticlhv.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/ghakutjvk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gghhivmpn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gleasrnrb.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gsxzbwcqj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsscxrnqj.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/ggcnhyeed.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gvutawyrb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gigjttcpr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gwvhcywpf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gtkepcrqy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gqjspddrq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gymdzdwse.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/geewtuafr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gpjrfsuie.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gcttibvpt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gnzralizo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghnubhaua.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gohogfggt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghpianhpi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvywaduuk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/glktgoelj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gykczbdxw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gevkxajkg.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gfzoegrvo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gwqdfzpqi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gpslzblbp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gdgxtxfuj.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghrzvtpmn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gagqfudbs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/grpedbuvb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gsnnmoppy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gnnosnppq.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gvbbwsobr.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gibklfmtv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/glkvywgjt.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gacmhmrth.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gthtiixjm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gswsezecp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gpsohoahv.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gfgvjwfca.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/grpkncogu.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gqzqrbvox.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/ganilxxsb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gdvnddibv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gczntmslv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gssyfwjfy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gahwgtkeo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gnfttetml.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gpgkmlnkm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/goaxndehd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/geakdiopp.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gqzhjrjhy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gafjtyjmf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gbrlmxlsi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gmvozzace.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/giqqdkuiu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gzkrdvswv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gptkiqhxd.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/glwkysgjm.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/glkrqsvme.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/glzsgfxmz.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gzhsjdmfo.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gwdrmqaov.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gqrblyjtj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gutslyaye.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gptrkookn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gwqykxngw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gterwpmzm.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gduvrjkrq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gbolvnsdv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gibrhemwp.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gwgpgxzbf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gkbqxtasy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/ggoxkdmlj.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gqsscnunw.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/grdgxmtxd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gpvdcthvp.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gzqpjqyaq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gwhqhltzu.sHtML


<!-- 参考信息 -->