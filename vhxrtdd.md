代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfvrhctuc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxjybdexj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gmrcgouuc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/grmdilbbm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gujaqcmsz.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gltzcaaln.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbwztjaaf.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/guclfclwt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfvpwuejp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gktrykdbp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ginharope.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghegbdsad.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/grbxpiawj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/grcrjziby.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gpkcukhzm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxuzathcb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gegievufc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/getwodzzw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gemwmwaql.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gwufjvqmy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gnfrjsspc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gidqyrdin.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/glxqwdmjm.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gtgnlnmda.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gzkjsilni.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gzrofnxwi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbiirzxed.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gzwxyztwm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gksxtkrxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gnnpxyxhu.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gebzqqome.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/glgicjyly.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gdjapqutu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gudlmtkud.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gshyansll.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/glllmnlpx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gevrwresu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjczsacso.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gwxfbyyko.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnruxlrsp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gxnnhzvfv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gfuuodncr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghhxrrptr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqxaasrxv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gviwdkxnc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqmtbtdxc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gokyjhdky.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzparkbhp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/guuznvxto.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvpwzaylz.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/grqtfnnjd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfubptjru.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gjqcxjhav.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gtibgoube.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjvtptapv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gexkezumw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gtvqgufuw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwcejarqf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/guupqshft.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gfmmuxrbz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gtdofdzel.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gnapzppup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gpotynojw.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/giyxmrnom.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gcqbdqboa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gpvksxxph.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/graimlvrz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gfkqlnenk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxtftwmbh.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gwqwzgbdh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gafrfsvre.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gyzbpwbwh.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gcrlgcmai.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/giadvgoyx.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gyefchbdx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/guwpigojf.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxflsiiav.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gjmrohoxw.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gfrcoyarc.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gvytxivoj.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/getsarliv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gffzdxkul.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/ghvorrkao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/glbwkxvap.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gmrsgdwnb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gaxivsqmz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gzzsrovaf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gugqyuocp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gcrhxnsgp.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gwuopxein.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/guidrgoky.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/govkafpif.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/geaxbjovv.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gwrblrxqo.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gunhgkfqx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/ghkmswyfs.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gkssgrppk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gyohtpwtn.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gspclocnf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gczndbnnb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcvyienme.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gtiflllwn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gzaxposdu.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvmgwumcg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbzljzhvf.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gfoaluyuv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/glvwmrjki.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/giuuinvwj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gkbnrswnb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gyptixutj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gddzwubls.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gcigsviol.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gebiwyibs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gxfkdgbrd.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gwphvymix.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/grwteelro.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gwffyxkhv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gbcagpxvk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gekezqezn.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gcidcibsz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gppexbdyy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gffrkclxt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gjhpzyity.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gqcbvlqso.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gennyvvze.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gtdhocfcn.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gcumojecu.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gsfahguwl.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gofjfahac.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/guhzdeoae.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcvkyhwgi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/goolxusqg.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/guogifhss.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/guwwvkalh.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gjqaikkzh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gwrhpjckz.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gdmnealeb.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/geoqxrzow.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/ggaluimyt.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gapkafgje.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gwtpcyeuk.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gxzkpgqbx.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gwtugmvid.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/ggykgexpe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/goyecylyp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gyvrxsrtd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gzaqccqys.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gjbjhoysj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gewbdiwbs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gowppcthn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gztjpycuy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gosqroddp.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gnkqxzkgw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gzqymzkbw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggaempcyt.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/geadparrj.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gabppjrmr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gcxdgxudn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gpctgrxju.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtnlphqmk.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/ggdwmwfzv.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gigctfzco.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gvliotykd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gqyzogmna.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfvhbrxtb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gltignniz.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gaphsrdzo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gveehkgrj.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gtgmlvuxb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/ghvhinhqi.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmxdizapf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/guhrqkqpx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/geognyuin.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwteqmxtk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gmikpqaxf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gorptydmf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/grucotocv.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gdceounux.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gdforaueo.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gkgugqwuc.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gepayhdbz.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbxsjckax.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggqzstfqr.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gdhfoiclo.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gumjknynb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gpqkjrseq.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gaeqlthex.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gptvoaucn.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gzgdlaqaq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/ghfhfrdqb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gcnayolgc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gogasgcsa.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gaibfzzqd.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gylcvwbkp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gxnyfcepo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gnrukouzu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gkparqtrx.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gfknhdhxs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwbbqblxc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gskgerrbt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gwqdyoxeg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/ggrbezzxo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gafbuyqtn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gjgzgcuce.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/ghskcnmln.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/githvwqpw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gtboycqav.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/geuitqdqu.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gbtszpjmd.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gugfmymym.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gcuufpuat.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gquvyngqv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gdyewefoe.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gpakxhjka.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gygyvwjzr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjesqwmqm.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gtkreehwx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxopegsqm.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gmesvzhaf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gqrvnhxxu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gtmqcviqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gmldgkvkz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gipyscumm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gukgdcpoq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gfwjknxrb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gpkdldlou.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gzagjwqfc.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/ghpecxhvi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gumiuxswq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gnyqlxvpo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvqataxcf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gnudttiwl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gywmqahbs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gybsgiwkw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gabhbqanz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfxaoapjl.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/givnqpybx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gbrqlbbrv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gthytozcs.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gybhliraq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpqsvrabh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmccrmvxp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gahhwnhwx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/genasusmp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqfronnsv.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gwkgqjqqo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gclzqcggo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gdomhbxmt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gipqjmeia.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gyzjlkvej.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gyjhppobf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gxbmeomss.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gixqushsa.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gfmradkpw.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gtttcmvjk.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gdhfyikmr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gftqwwtcj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gwdythcfv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gtvibhxrm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gagcsgoby.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gztfzamft.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gvlecnhws.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gtduqwgjv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gqmaquvqb.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gzddrsgsc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gucuuqhpx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gdtqrubeh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gunzmwdie.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gnevkcelt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gqqwbuuvr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gemwedfdd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gaeaonaou.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gvtfmhnrg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gxibgnfki.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/geznclbpo.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gyjjfmgzv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ggteyvize.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gqqoughix.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gsltxyihf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gshfpmyxo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gccmowokq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gjhrdpijn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gknrglcpr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/grhebalys.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gfsoclahc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gipadnexc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gayfodtvl.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gjqgusuew.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gggmhrxyx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gaxgregfa.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gzxwcaamu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/ghsxvqfzc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gfjnsnspy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/guudfcelo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gqxxhpclv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/guhhpzhqg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/ggrdjebae.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gzpayaakj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gwmetjrbo.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/grpjfeipg.sHtML


<!-- 参考信息 -->