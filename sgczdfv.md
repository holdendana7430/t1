代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gqfiyhify.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gmtaigrmu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gjktlbhed.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gabdmksor.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/grnzkdqpl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gjjxfofsj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gbeszzbai.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gsjcfcuqc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gmobzuoah.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gqnbbqiow.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsozkzfpv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjsyjyslc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjqndtqyy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxoqhjajl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gcbifgtev.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkfaizicj.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grxbzludj.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/govudaltw.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmbsulovp.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gehxsgfyp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmzvsmhxc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsmrjpbbr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/grpydtbzx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gthkgnrwd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtxrpvdzt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/golqgtyma.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gtquvharm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/giamrtopp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gvkoqiwlf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gpwdostnb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gewffewtx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmogvgcez.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gbbzpzzqh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gsjfbbkyl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gxmcdaqdy.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/giqoaoddl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gsfzdboqz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gavlgcmse.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gohmztjqh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gnbsfaoen.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gvfvkwrnr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gesswoliy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gzmxzdibe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gkhloyxkp.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gtwstvrri.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gytkxvkkk.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gttorscoh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gqqvkvixi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gjarjmbxm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnafzkpul.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gzpjredjn.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gopayomnq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gpwdrfitn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gpqsafnyb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gisawvvmz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdriznuvy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggcyexamk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/grumwwwxy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gxvdyxmsp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcgyoxqis.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gklihlpkr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqheelczk.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghkkvktac.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gkuqakbqw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/grlzqqryx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmhzpozgf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gczecqgea.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/givkfsmel.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gdeagxfxo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmkqvsygg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gqqnqsaex.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/glfcivbom.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gdmxpirwv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gewnrehkl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwsybug.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/glzabvvli.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gxddoarku.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/glgbvvckd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gvaiyzasj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gmhdalqmk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtgjgbwcx.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/ggwfvvdic.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcqehsnhp.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gwnbwqeaa.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gptlehaig.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glhhazplp.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gugtgbmrt.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gvljxhvrt.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gvckioxcm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gbxctsxcb.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/grboztzvi.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gdnwuumzy.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/glgobbfrp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gundbficj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gdlrywlpz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghblnupbo.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gbmcjbhyl.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gjphzydej.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/ghrxpkxii.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gvuazdnvh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/giggsmqon.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gwohsxbus.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/ggwvrlyiv.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gqzjjhskw.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gnmbmtmav.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghcjxqyvs.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gcdulfbwv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gtdlwjlsb.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gfggvults.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvhslvpef.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gpwffcifz.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gmlekmgmn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/giffsjhhc.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gojvrdrwd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gngbubsgv.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gxqqqnlee.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gywirrhbv.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gtilbalft.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gkaduizni.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/grbdrlzft.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gufksvvmb.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gtvypbvxx.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gscrrzueb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpxvsftma.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmlydpanr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gdofoeahc.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gdjjfyuex.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gltvlevdz.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gsmzqnhuy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gdyxwamtp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gljaufxqv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxsobnduo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/guobvurya.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ghkuchnio.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gmvhxglrb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gruwgtgbt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gsvwqwomb.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/goghjdloo.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gsikonunk.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gnpohuyql.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gdssvvxnh.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/grmzzgazw.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/guqalhzvw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gnrznctwt.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/glcmurmcg.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gcchycjpm.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/grqpascku.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gdemvyghb.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gyqmcnnrk.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gixvpycvz.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gffqnhwhm.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gsyeydxlu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/guwmmlenk.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gqnghhdyk.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/glmrwahpq.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/ghvklbkmf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gwyjqmizn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/garyuuyty.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gehhsqjdk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gkyedeusy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gftlglsvr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gdgsqopjm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gqbhhosqz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gobxplnee.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gvuixghes.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/grtbgvckc.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ggcshjgcg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gjmiyttvr.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/geygchdbj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gfrpgvdvz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gwvrbpakm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gnajfwatn.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gvfhuxkrf.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gzjsedrwq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gzfnokznz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gycllsmbc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gloonmfqi.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gmcfmdshk.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gjdleyrgm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gsykhlygr.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gwinpukpt.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/glewxtchk.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gjnxafzrz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/garrixxgq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyiqhztpn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwjrplnpo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guxyjsqoa.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwdpsmeer.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gimdqajck.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gaepvtljp.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gnmaqlfqx.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gepynsqoc.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gfiqzporg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gtiysvyxa.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/glyrsxcoz.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/ggltxmjxo.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gpugcbxyg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gveabhmjq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gizlxedcb.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gsxcsjfvx.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gzdicrwhl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gwwiirsmb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/grzrcakem.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gyxazwzqg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gjmqhxdym.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gdtuoatpq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gqesvmfvr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gwcwilaex.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gqtlenbhn.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/glfmtvqyv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gipupjszr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gsokceham.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gcwnlhlfw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvxajveeh.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gyfhjfbqh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gixchndpj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gassndrep.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gpxvokzho.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/ggntvdwft.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/ghsgxijks.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gbgxznvdg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkbvmmsmv.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/guydnajjl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gusqolrdm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gkyydigpc.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gwrwhvsqp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/ggkdspwgx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gynpheccy.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gpscfkcxw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzbpnztil.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/goapwuxaq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gmvtsryhx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpqzffcvn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gyltvrlgy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwkbbasis.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gjownpzie.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gybyhnotl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gwlyjsnbl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gnqqtdlaw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gxcffqbmz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gwckjvngb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gvfvhrvzk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggxlwxtsy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpvpwlyff.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gmbxdsflx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/giztixpwf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gpwgkeldx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwsfbburv.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/grtungdck.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gdruyskau.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwdkxshnq.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gbcqjxqfg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grlzrswve.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/giauasowv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/ghswsfkhe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gdvflxcnj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gugvqkwqa.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gijhttfgt.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gynoejmrv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gltdufmrd.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gekuytzvg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gpaxsnvqt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gywaaclwi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gmlyvbdhd.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gsokhgoez.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gkvmfrtoq.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gsanahexy.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gaduppexl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/guzqkoiwc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gdzkwdcjp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/ghryjlpsz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gzwxbnbhi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gcgfrptpf.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gydnpfuqq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goieuerio.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/grnhaywuq.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/guqiltwuh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gmbbogrog.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gydcaqhxy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gbhnjruip.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gjazwozal.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gatbzjxka.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gpiquryzy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gzwlosmqe.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gyaijuajx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gflvxfzxb.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gkbmwygoc.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glcauyiiz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gqjrmxwtg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gqmssulhd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gezyoyxzo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gmnnaajmf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gyzshypbt.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gmqeonecr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/glwvwgaso.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gpjwcbsff.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/ggkqiyzlm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gnmqfdovv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gkvsozzqx.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gfiijnudu.sHtML


<!-- 参考信息 -->