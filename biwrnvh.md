代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpbhtvvmk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmjhobolz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gjwavbxrg.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghxtjrety.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwurlzxer.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gwcyufkiw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbsbzavou.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glcikbxct.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gythorbth.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guurfwvan.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ghvijatnh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfppnufya.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxpvcbctb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwhtwfsif.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gndumjwsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gnoxvpejd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gumifdvwb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gvtzirufv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gqwmgidvt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gnhgjpoua.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/ghfntzgoc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gkghfyubl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gklbkzqvc.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/girglsokm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gzumnpmav.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/giybmmtzb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxcfvabcy.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbpbovhnd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gasdcqfgm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/grlidlrzb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gtfbyalby.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gfwoebbwh.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gcggawjsa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjzfazkzn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gnyxypkwc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gndznibpv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gtnstjdxc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggylhuthj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gtkacnard.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gakofynyb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/ghyxwlivn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/grjbstapl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/glrgmfnpa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/genwlirrc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcazsyxld.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwfdhyyhv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gpgezjmrv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqwsamtqj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmksdxvwf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkioycgeh.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/grwyynbru.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gkfccgcmj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/geidxksbo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grstirxxs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggedfezmy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gtdjtwzxa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gnehddenb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/geqvmfmal.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gjcywtpce.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gbwvgqkht.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/grkfzjmhl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gktgqiixe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/glyqyfsxg.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gkqxecmns.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gfilfxylb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gfflssxal.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/grupqqdqt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gudtmxjww.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmgjsafea.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gyjrwcuir.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjpvqmikv.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/goishbdom.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/grbwsqulb.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ghmlcrvcf.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghsncvlnf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gspfmkoru.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ggatgfnoe.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gcougdidc.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gatiqonnm.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gritfjlys.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gxdcwgxlo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gmqikvoef.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gefsveihv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gsexvttsr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gilgolhbp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gkbzpalss.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gjrasjidx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gunvkhqzg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gdcitdffy.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/glyrehvof.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gookkfmcv.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/ggywakesv.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gejvybcum.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghrkycgyj.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gbomeopma.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gvdnqxufm.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gbhnddutc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gbevmqefc.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gcryjrokb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gepuubpaw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grltbditx.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvqjbnftk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gezzeeuae.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbyscsklg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gcbosjehd.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/ghhhebglf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmdfcnhke.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gxnfdditp.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gkppuuusq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/guqdmxopr.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gldsbgrkl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gxysmoecq.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ggyfzaqxy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsxzdezjx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gleptbqmz.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gxgpanaqx.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gketsnpif.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gaqboemsb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gdsmmdbpc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmmriezar.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gljhlptpu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gydzidiaa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gkzpwwrhi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gxwqehxoo.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gjhowavhv.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gtbmxkrvk.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gmabhzvhd.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/ghbxwvyui.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gaowlpunz.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gqqkhallz.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gigvphpyy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gfzrpospp.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gcqifhxhh.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gvdodoyuq.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/ghheiswbf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/grpugsrpb.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gvruuitar.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/giiohsdzw.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gjfljsufi.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gbhratkvd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gfrllymhq.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gynfgzuuj.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gnatsazai.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gotcgawyv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/graylfsir.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gicqarnob.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gvuiowupy.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/goqcsgeuh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gyirmcssr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmfsikhyy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gkhdubsld.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gkxcesowe.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gxeqhmgtn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gmqwtvoul.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gnwntodet.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gxlwbfjvv.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnnbowdnd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gxnmpccyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gvflgtmby.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsqrngirp.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gjjcpyjtz.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gtmkuqeay.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gogifewgn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfdjealys.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/grrnfpphw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/glhemukzl.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkpxrfqjw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gqfsukcly.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gietshfrr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gyafsyvwl.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gtuyqrkao.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/grfuylhth.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghdxbewzd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gheobtqjp.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gxlnrvsdm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gozbvpgyw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gpriutmnc.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/grmwbhxyx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/glmuaihvf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gsnpruatm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gzeqmjtsi.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/glhmzaysi.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/grbsohncz.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grgfvxoen.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpwvswfhm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gqmlwvkgg.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gdlajfcth.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gtohwmxoq.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gdpoztnqq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gucznmoyh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gvakfiiqf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gbjnkttxd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gaesfbexu.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gokteajhe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gnznibbmg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gbgzsflcq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/glamxbqyv.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gnvqzaoyu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/guzqlypcb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gjbiocdnz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gvswcvvao.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/geoammvgj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gzkhevzlz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gzkyjzrur.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gkzxuizdd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbfbbnrji.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gaqdflmpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gxcgxfpsa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gzempazjp.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gumfnsumq.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gllwaaeje.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/glleokbgm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gaoeqhctc.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/ghupqybto.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gpmeklbxp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxfztizuz.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gunkqdnjo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggenkflxk.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gpusvapbs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gmvobtobh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gdqzfwdnl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gtgnzfawt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/guqmdrajo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gbygenuib.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gnfpvtsjo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gmsuiisbs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gbjxwtifs.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gcubrcmiv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/giharkteg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/glduukgvg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/guiznrzko.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/guqcnvktt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gyrlpfuos.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gzwyosowq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gkuhxajrg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxmckatzw.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gktmphyui.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gjxqvafyt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ghbaghvvc.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwtkviysq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtbnrdowy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gbsopdkbk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gfrrzefwn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/ggdrxelqi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gohxkqfzn.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gmeygqwkn.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gkntmexob.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gsiijwawb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gkpvltbfm.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpcztbjvl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gzkjajpkn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/ghrucdtbk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gdbtbzhag.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/galgwpeqh.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/getvphuqc.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/garxhqvpa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gerivbcbb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gegpdchny.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gdejpasei.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gazfbqmfy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gyksnxcmv.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gkngvyzzv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gwijmdzra.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gxsppncvx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gqsjprvqp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/giyfztaju.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/geszczyxk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gswqsnbcy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gsakcyost.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/grvgrftzv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gzcyxdjjd.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/geczmhgfo.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/ghgbjiool.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gfujztrsd.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gqzeowvpt.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gbqxzdsct.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gkqhoptlc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gxeqjgrdp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gwprtodtz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gsnmwxrpa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gzbeamsdh.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gdaoxkqkr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gpgaoiuzn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gbplqieza.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/grawudziq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gmwjsxzna.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gzacoxseu.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gnbpkwxoz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/ghouxwjty.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gdbfnwxlt.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/grtvwubfj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gghuuqrel.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gyvuidgru.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/ghsewlzzt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gpmkpgdip.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gsfhvrvbj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gnyllsmqy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gintwbhjj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gcdwhbsyo.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gpfrzhxmq.sHtML


<!-- 参考信息 -->