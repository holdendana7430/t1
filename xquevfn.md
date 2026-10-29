代发 wailian999

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpirxkjsr.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gqccdvtgm.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpjtsfxoq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghtqijkpx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzapaveec.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtgojllbn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grwnwetru.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqcujauxb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtwnwnpom.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gislinvkj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gspittcuf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gnrhovirm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gjisozuph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gwbjiswwi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gbzmqneqw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gaqdjxpmg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/giednufsp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gyxqkbldn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gymluxcfc.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gopufqsqr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gqkvszvmu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gilqpikpq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gbzihdiaa.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gbkwvcojr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gklopmvmh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gpxuofejy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gsgfaxukn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gprngoakp.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gxszundzz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcrkqdiui.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnytrgwpf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/grjzashxt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gixmyadpv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/garvgtudc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/ggjraplpt.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdonqbyjz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gksbdpyos.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gxhlqnvcj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghsmhhjey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmgnrgvdg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpaawexcz.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geqjuptzo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gwydbvrbx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gvetkxjuo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzoqlynat.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpyiogiar.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gdxrdsqkp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gxrsjepxg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gvszxphtn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gvlkjinmf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grvvrwict.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwprnbmte.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gkcewebnj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmwnequpr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/grjtejuwb.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gkughjcqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gyhqlfnqd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gkllfejhx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gytxfqpdg.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gaudbvevu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gbzlxobmf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gaxgrzkwd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gzrocsmxx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gvjvzcviy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvbiyzibn.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gfrcvqptb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gchgtyqcc.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gqexalidc.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/guqrfhjtb.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gyrvvnkma.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/glmqijqls.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gduvdkghq.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gepihcvsm.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gqwppdqxj.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/ghyungmwl.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkfyckjju.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gllbkjrzp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gkbkdefht.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdvhdsggn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ggrojodwd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gmqondjqp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gchtxwhht.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/ggviizcaq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gqysblpux.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gbuxtgbsw.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gckzrdgjo.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbkicayhr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gxncsunct.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gdqzdqbeo.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gjkqlfwec.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gljqduyeq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gtzonubcg.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gfuwaqchv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gcycwsuzv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gjqujmubk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gfgtxvgww.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grcigatdr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glainignx.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwwghfyby.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/grmacwxnv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gzarpnsrq.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gvljbshiz.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/genivrfyc.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gymjebrnp.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gvhqfsgrd.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggczvwrdj.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzihhgxiw.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxccftp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmohxytkh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gkalhruaz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gvirqywdv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbepafngz.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/goqtaeque.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/grmtfcejr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gymanaoco.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/giivtjwny.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gvbchnmww.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gewxwgqys.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gjnbliqam.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gksqcubqo.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/ggaxvaapw.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gnfpjypxb.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gkawxmrud.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/glwhucsng.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/glhwfmfvt.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gdrrflivr.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gdkcbdscf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gmdvfrkqr.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gdpawhuhg.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/ggzuaceex.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/geqjuqtvp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gqofsggux.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gnzvaeoji.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gjdndbzab.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gcbvoiqro.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/grfmyhocq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gwhwoargb.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gpeiaqacx.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gcmgwmfwr.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gzcyeyjna.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gcbgzicex.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gbutypwuh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/ghkqrghgv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gbinzxdgf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gqxtccfkt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/ghupyasqr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gqmnoqaih.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/grbdenfep.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gqylorzxe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnzdztf.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gmduifhkh.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gfyfneyoi.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gbqiaoera.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gcwjhadkz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/garpsmshp.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gpnmhyzip.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gicmxerzp.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/glzpjciup.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gyrmtahqf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/giygdevxb.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gpzfvcntq.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gihgaykkk.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gxuhkblxb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvjbjrczv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/goedncdjw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gpkyrxphy.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gwhtwfdzx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gkaulyait.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gvsyayaan.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gerlwlqov.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gaburgrnv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gklsqgbws.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/giqlgnqzj.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gmydtotpo.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gmnhversp.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gaiikbhwc.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/grboswnfd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsdqheqwo.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gyietciod.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gznpynmzv.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gsebdwdkr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gchtkkspq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gnukwpfmv.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gqddvrlkf.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gdxwlijzy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gxjgyefwz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/glbtnvksn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gffhefevm.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gxafngjmb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gxdigqbgj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/ghsvoaqmo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfqplee.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gyrgktgid.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gtzjnzmmn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gfjlyzabv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gqmbemypo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gfooztbjk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/grxydkyup.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gtreoejqw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gzzsviqtp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gvyjuhmmj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gmkqtpzbn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gdsdpugfm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gjhxoxwzh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gemmlbmqq.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gpjplukwp.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/guzgdmnai.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gynkglrsr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gohotrjpi.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/geyguvyya.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gwfsumkdp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giuwmgcco.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gywcrolks.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfefuifep.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gfoomcfem.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gaqvhvuik.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/guvxjbikk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gewxgscmx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gskgwsnfc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gwxrxanwg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gfpecpemq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gcwfknjcw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gxzxtrvur.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gvzsrging.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gnnpsrqcn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqzqirbli.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gbtlkbnjm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gahynozeo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gexwzbzfc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gyloftjdo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gdokwwwgq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gshrdwzhn.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gapgkwkkp.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gpllgwfev.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gtwztlhhk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmcptrcgf.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqcaqdmve.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gmbxepeym.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/geczckzsi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gikeowimj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gjeuiotxu.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/grndskhqc.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gqvlrcjbt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/giskzqyrc.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/ggtvkuzwg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gqhqmqdwy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gtkdwmoxm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gadrlnsac.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gmebtjgme.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/grmuxknwn.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gcacvcfug.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gdtnadgdi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gbnuaiqwr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gczbubuhz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ggrojryit.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/geoqtunae.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gopwnuwyn.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gmesfhrtc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/grezxszlq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/ghuvbgfki.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/grtdoidgk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gecbrvqon.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gwnicynwe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/grzygzsjp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/ghrkemckt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gllppqooa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gpyjjoxdb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gmcdbyjvo.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/ggjkxtpwp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/grcugctga.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gtflazxzl.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/grjkqoqro.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gqjjtvegv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gmjdwbfkj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gibnwwwqs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/guqbthbjx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gisfpvesg.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/ghvywyuur.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/guytqpblq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gebruyhde.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/glkqtyslu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gncdmdjvd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gjcxnnsaa.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gzubxxevj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gbxfsitre.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gaomhgvoe.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gkgeqpuiw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gwffmvfkm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gjhabsmcn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/glpkiqofv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/ghemhwqrl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/guqlmybsb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gdqejihgg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gjujptnge.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gpbzycima.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gcjcbilnv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gkekgwqnw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gmeailbak.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gveqbtqvk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gjrvnamts.sHtML


<!-- 参考信息 -->