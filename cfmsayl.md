代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/geuiatudv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/grxwejkef.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqtpozbs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gfefitrpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gwqloopdl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/glwoyzvle.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gmsscgwlq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gzvpkiglp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/grmmemxci.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gjpnlbkri.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwkrlbeyz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gszybgjik.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjvauzbgf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grofnxqje.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/goodchqaq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gywbxiexk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/glsvykoyk.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gqcgrclon.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grotybmmh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gesondoih.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcrpzrxql.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gouyqshlw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gnpuioypl.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjvhjryxh.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gihavjodd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwdhnhrdv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gczooyzsy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gloclwfgt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/goqnbwqub.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gpzgyydpj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gmidotufo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/ggxfojgmc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gnbcylogj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gdxlywlhu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gjghvoptr.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gqfganplo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gflgafati.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gmxqzjsta.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gdubvvlqn.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/glewnwche.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gmwirlxjs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gaoplunzj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gccsegadt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gspqhcbpf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gchvurwzl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gctpmrrxj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gvazxijyr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gwncnacze.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gctvqkquq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqoqdtweq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gwlzezsni.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjrsvdoz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gxveyynsl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/grpwlixfc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnnbmkxy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/giybcncib.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggexbykjz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtmsaducy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/grrilnbaf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpkrzrilk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfpwensak.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gtesfhgjg.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/glefvhlxg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbrtnsrjx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gfmeiwlav.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gruuwyyfw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gsclhyvvg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ggfsaezum.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gjlrzvrct.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gnsuuxsrl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/guzbrcamr.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gswmpmclm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gjlnpzcsj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gcgloepsb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gvswzfzqk.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gkhzapbry.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gsqwyghqf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gfdatkosu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gvaebizvr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gztdjxqmr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvpocosto.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gfntwwtsj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdnedwean.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gmzlhuzdy.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gzajjvhcc.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gjnsxodwk.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjalbggcb.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gndlhntne.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/guhydoaeb.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gyosjogby.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/glkjwnjsx.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gmwgjxjne.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gpgxefjuh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gctedfihe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gxbrexsdu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdyownuhw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gapvpiruh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gfyrrynkj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gazsswldb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gchcpwcsw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/giuuqtrsg.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gdhhycqjz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/guzecwlkc.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gbypfqqfe.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/ghpuzttsz.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gluwmvyfo.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gptztmpli.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gfpovvlbf.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gjvxlgtku.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gjeabigwz.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gsadtcptk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gvfhbykhs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grgxcutmm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gfuzsohbv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbfxjevcv.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcwyycvbh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gcwggvjho.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gcikrrxtk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/glybwtvux.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gmxgnrald.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/ghlhjbvud.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gpsfbgjra.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvwpgawrh.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzipypsrb.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghozrkujp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gutsqnnbo.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gxctnuybm.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gtqlikrfk.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gcqofsexe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gmquvirig.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/garakzobo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwordyclx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpfktijs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gkyoinmrp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/grixiuabx.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gmmijmlpb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gvxxwdjgl.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gadmdhotf.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gicqbhpvb.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gpwagqzcf.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ggeznciyv.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gttwkjlph.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gtmhwqajt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gkqwbwchv.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gkpivafdi.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gylcemyrr.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/godjkyxtz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gpjhmikrv.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gupnrfyag.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gfgsocwdn.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gagjkglkt.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/glecsdkwt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gwevzmtln.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gkgsthaeh.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gbomzkxcd.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/ggpvivkwk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gzhqhhtdg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/glxevzmbf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/glskjlafy.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gajrfrotw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsfiocjzu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gvciofsjk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gqlggxhnc.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gfepyyffu.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/glmmjwpnd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gyrnewjfg.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gbuajhdjr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gjtxiwqpb.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/getqzodkq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gwcklnwir.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gatlanqdx.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtumamtja.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gszbhlyhz.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gswliqsby.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gfptxpczh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gqvlykpbc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/giuthpotc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gfasogluw.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbuvsmslp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gwmkgabzd.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gcacnqfvr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsyvpehh.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gzljxojzm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/grldaoszr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gnwzgcfgs.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqkjqxiap.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbmjfufro.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gxqxzsjxn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gdzqmfoxy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/ggtsauaaz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gwlqiznlf.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gpnnjherv.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/giaovsieo.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcwrsow.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gnmlfdlum.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gnpfxntxe.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gaxsazdvf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/grzubnvzc.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gwbvvxpih.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gsluhefvw.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gavqnvypl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gglplqxkt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gosgcqwym.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gscwvtooo.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gvnslulmq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gpzeueuhz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gixjbmooa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gdjrvqepl.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gdzuwnivh.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gofhcfobs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gafdjmnlo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gcxsjyhrn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gaoaoajvh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gucpmmtif.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gmoavuzlw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gvmouraio.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/grlgftaav.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gypopfhyn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gpxcezasi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/golcuciuc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gubetttua.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxadyozvc.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmuicddim.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/goeiqzgxv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gaxbhlkps.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gwiwpecel.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/ggguktsgp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glonsweom.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/glvkfmldk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmcwnmeqa.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gcwlraffw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gzjdkfswf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gpghbkpgy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gvheldgth.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gphlsouqf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gbfpfkpux.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gvarwsfcj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gjuwjigpv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gmsqwftqk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gdgjtmfcs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gemnjncoa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvvhbeady.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gewjwdzil.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmtjqutwo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqxhinahy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/giifhtejo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gixuicsih.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gaohmrjic.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gmhwtcsgf.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gvnytqvtz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwruqywib.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gizckrjvs.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmlbjzopc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/glwecimar.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gysrurqat.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gyctqqdsq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/glbapcuca.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gsirtuuks.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gzscztqfv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gcdqtpblq.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gfufygwop.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gojgmeyef.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gwropqndy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gwtndizok.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gpdknjacb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gjzwjddfl.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gvzdghmsr.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/ghobzmtyp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gtxexdmnn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gxvejgkni.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/grjyoxpqb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gbtzxmfyd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gspgccfgv.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gdmtzwtem.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/glwkgjyqt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/giawbhyxa.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gtttjefaq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gbastkftl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gdbqyqlei.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gkbmtdczi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/grufbubkf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/giuadwpji.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/glrbonwsy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/ggtwpemii.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/goheuezif.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gmzjscmla.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gjgghqfkk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gfqafphgd.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnceqrscu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gwwwxzbaj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gyxvfwtod.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gwawgyona.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ggztmxjum.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gocvnwpuh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gdzecefxe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/ggdshxavq.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/ghqpudafl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gczkqfiyz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gausyoctr.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gdfzllgup.sHtML


<!-- 参考信息 -->