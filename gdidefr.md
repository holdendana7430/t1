代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/giylomgqg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/grbtpfmwi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/ghztrmdjz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gslslsdir.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gffggnlhk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gnqmnwkpf.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gaozhzipz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvlqgmb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gamwmrtju.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gajphewgg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gtodjwcgm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdvqjzbsq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goladxxgp.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/glpaurizg.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gauypzxom.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwqifplwm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdxszfqzo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggaofudsa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggijcnzqg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmlrakyjr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpirpltwq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkpqdewan.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gzkqxnyot.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gqftofkmz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gjpjltceq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/grnfcjwzs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gikvxvyyc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/giwtsnzmh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/grjkssjhn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gpwwmzvnx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/grobilmlh.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gsrlbcesz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gsfciydza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/ghoqfqako.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gucuobqhz.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gvmszcvny.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gjtnlunpn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gfgxuyozv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gvtrsievn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gllharart.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gydnpersh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbwkwwtvz.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gnwbrhird.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gybxtuufz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gjqgaqfic.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqilznbhu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gppwamnfc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/getdazpcs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gazekapfq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/glxvfzlbl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/golhueszl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grlfjzolq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcizshkcg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxemvskwr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gonmgpbni.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gdstyaasi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbnnfauti.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gupjnomaj.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/guknrpfps.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gttnsouej.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/glzkobnhh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjtdtxqv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/goyfxurxy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gfexoxewj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ggfqntuog.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkuafmzqb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/giinhurki.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gnyxkcxzb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gxkcuihus.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gyadlvkeq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gkhctpmym.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gqduooxtg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gkimynzfv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/ghnxpzsbu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/githxnneo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gwclmpmzl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfpcerlqv.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gdsghtkcv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwxpdxgne.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gycqsjhye.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqgbmjvsf.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gkbngoydh.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/ggyqqjflu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gutuxezzq.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyrnxobrz.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gsqjzqlhe.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/garliyqdf.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gxbpljdxn.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/ghjutrcgg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gbbsqvicw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gtnfsrxfc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gctwuzzpe.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/ghkhzbjpd.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gcykrsvke.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gmuxeoupk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gmiekibfl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gbvpqfbno.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gtypghapz.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gcqowmalk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gfqojkzqc.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/guikigclv.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/ginptdkwo.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/guufrrljx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gzobapsgp.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gyuozlgvg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/grpmsurii.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gikiqidty.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gdbblpygd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gdiftzlby.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvlevjipj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcurwkbeu.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/grvdptzoo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcklqsero.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gleatohjn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gzpvpvite.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gzmxlosyi.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gpqaemcid.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/giajnfqzt.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gdzusaipy.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghjguoatw.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gymeyzdoh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gkeqrjyoq.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gojeieiup.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gfjcnifzs.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/ghpibmzwk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gmbopbmzg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gecmfxlwy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggwvybaum.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwosoycig.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtwyfayce.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gxolajelp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gyxawwfrf.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gouartarp.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gfsitjqns.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gkyxfroau.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gujutwdtx.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtlukszji.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/ggeciqejg.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqnbazhec.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/guulmjkwe.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gzcgemzmd.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gqeaiasut.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gwwuulcec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gbncoshmt.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gpomqnjss.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gokdzivyb.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gqkoypoch.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gwqzlqbuk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/goesyfftu.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gowxibcsq.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gloyvywnj.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gatgeeoig.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gyanwgeky.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gqrawvmxc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gcrqzjysn.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gvtfsiztc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/geomwqmnm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gitfjqubv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gtgvbmmgi.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gkfbcjpqk.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gdjpmebhu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/ggmoxbfts.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gujxxleln.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gmwgeyphw.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdshmmago.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gdgxwmdxa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gseugcgbx.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gnlvsists.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gmhkdikhm.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gtqupinwm.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gwzobvdey.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdjkqdly.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gocwnpwbc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/glapsuxiy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmdvnhnsa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gldxlqcta.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gutqsyozg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/ggsldjylk.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gssjbvciv.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gamyzzcmv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gfbtyydsm.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsenesbv.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gftjgfnpl.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxdxjccjp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gvrsijzhb.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gemruzlib.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gdcvbfgce.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/grulneshl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvtrsfeiu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gyldrhxaj.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gsqrqnjev.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggzgudopb.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gfyvnjhbl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gpbiokekc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gkercagja.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gfxjnrtwz.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/ghnzflyyo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gqkcrqsqh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gtavnbltz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gzwtovzaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gedyddrkg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/grmvsasoo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gmyjmozko.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gkpxhubul.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gbdbekhac.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gytvmlopj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gsvfytokb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gncrczfze.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gykcnilro.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/glipqixdy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gyfxwymha.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gyxlestyk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gyucbylvl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gbfijslqq.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gooieotwp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gfssdwehz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gxkseerkg.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gvxqgqjct.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggudmvdvw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gpwjgoyij.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gxzkkawjk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gafigzpzp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gjwpemwva.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giccyyxhf.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gfulhitoe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkpfjwszn.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/ghqiqxncd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gafpafqls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gaxolbjqf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gwpmpcgwn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gaairczfe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gjkwqucst.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gpkbyunmn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gomkrbwee.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gwjhwhjci.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gqturmohi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gtecvgffa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyjpqtbnj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsgzdngvm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gphtskusd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gyzsobnbk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/grfqcqhwp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gzuwydphm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gdkknnsao.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gtvgduozv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/ggxfrcgdl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsaajmgnu.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/grndsizhy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjvqxpoif.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gvfhbybny.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gabyowkhx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gbxlrbykq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gnkqewiqk.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gcqnqawlb.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/geqficesd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/godfniiun.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/ghpolnwhr.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/glldmjliz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gduaxwrib.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gmyacraru.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gkbjzedrj.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gsxwxbgkf.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gmjbxdkok.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/ghtqnftof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gxnsvxtmb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gkuzjfdze.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gkmdmdjky.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gkympltil.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gniskwzpq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gdomsecio.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/glxnjyjix.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gjesosamj.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gmkinpawp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gpugawlsw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gohjzqgkm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/guhkwslyf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gbyfsixra.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gtshhgabi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gbstxmqdv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/glvftusib.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/glhsnwocf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gtgmeqluf.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gbzdqqihb.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/goteskoww.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gisajbiaj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gpzyzclix.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gzetynjec.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gimplddkk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gyziciajf.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gnpylverb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gzholuunn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gbkwoqcqn.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gazidmscp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gxggsfoaj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gnevnyppu.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gsunohzvm.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gffeowxka.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gchlsvgkp.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gkdkjwlxf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gusjdoztf.sHtML


<!-- 参考信息 -->