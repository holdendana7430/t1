代发 wailian999

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvxwvlubd.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxjejqcqz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/ghpzcdrhk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/giqtgguoo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/grmvkxbyd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gjwmetzak.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gnrycaucb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gwybonmvk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gtyekouvo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gbdkfnrnr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/glgnmficr.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gtdwfewny.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gabjmikot.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/geypwqbmw.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gsbytrwns.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gvwfkpurq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/grxefzbtm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gsonrhqvb.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/geemqgcdd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gtiqhhrhb.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gsuitfvpk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gibwuvckm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjqmluonc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/giijcyklp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gqokbhpnw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gtcdvvveb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gjefnroyj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gseoenqou.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gnigmgfnk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gpmvbmkwf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gynulnbhk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggphovwcd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfflumfmh.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpudkisjt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/goiewtejn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gunullcch.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbxortzkq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbliqmcla.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gvlrmvfod.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvagqkxiw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gxbedeeha.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmlsyczzj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/giujavcuj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gmhfgwxvk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gmqevrqpm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gagkwwjad.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/grpnjtiqy.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gbrnhvnet.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gbyvubbnh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/grgffhepq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gnlxltexw.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gummyulxd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gpicztwkm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gzdpkvrkv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/ghjajzufh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gsxgqaqin.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/godaoowib.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gfgincioq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxuqofybs.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/geyvupklu.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gsubcjjyi.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gxobfvftb.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gefwhzhgi.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gvjxietga.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gpfqgpvbo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gqhihyuvu.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gbaboivkd.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gewozfmbw.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gjhfnnnxx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gaduxxpqz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gbepkolfz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnwwhcok.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gmstelruh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gyeekkejg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gyuaolchf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gcoienrwy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgvipgop.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gvhnhkzqv.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/ghoryfnhm.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/ghqnrgusr.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpnltaxra.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gfbysyonm.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gkzhbvkjy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gkljjwzer.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gklzvvykm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gnvfkdgue.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gfmncyjpk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gfmruitim.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gshwpisnb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gyffotrtx.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjdskommp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbkrrrgri.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gmdnxgueh.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gqbpkycbz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gtnpakauv.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gibobvpew.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gjjyfkbch.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/grwlmerui.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzzpitczw.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gouhqnout.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbizeltlr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gdjhjbhjy.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gbneasisj.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gzjoglvuw.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gjbclnmwh.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gnedvztqi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gijuqslwe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwuzudjpp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwrqrtlvu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjedyyhuq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gfrreriik.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gfhyygthq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/glkfrgcrq.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/ggbjqlvkg.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/glwvrlztz.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gfcxrdely.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gdsiaorlg.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gapyavjwp.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gaifabmqo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gkdpbkvpz.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/goklonkhi.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gushpjcyd.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gplmwktof.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gxewojxll.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gcitomszf.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gzefgyhbv.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gowokftng.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gdhzylhke.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gusncqmwu.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gxlevlpdy.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gkpreuyxt.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/ghzzzrlrj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gquqpcttt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/grjlrviwt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/grgrijjkp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gvbultvuk.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/godvqnklg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/ghjwfdnkt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gitdrotbf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gjuyyaotp.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gohkssqcl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gkquvwubc.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfbxwrluh.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gaoqueqnd.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gevvzumob.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gbfdqpqwi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gbmfgzkmu.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gflndbdya.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gyklevdbl.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gmjvketvu.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gkuznbuun.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gpppygeqz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/grbyfahum.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gqkvokczn.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gcnftzfgx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gmkpigqqj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/ghbjvgcuf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gmgxdeqxl.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gtcpsoaij.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gpyogezas.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ggooaarkv.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsprpqwgq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grfwzhcti.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvydkrvbt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gylbwyequ.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gknnukqtw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvvdghggw.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gxcqajjac.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gkvogesxm.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gtzsabkfk.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjmpemndq.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gipdbjtcu.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gartyqsgk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gmksajqgw.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gporwfxzf.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gmrrwjrhh.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/glxcypksy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gsgfvylab.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gwabxwyjq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gwsqimvop.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gddsyfkoo.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/ghhzlmgwq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gqmhdbmgr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gxfjxuxzv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gtpkmpidt.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gubdehajl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gjynnagqg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsbdpibgd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gckqnvemt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gkkzhvoee.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gflczhtos.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gdafzaczz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gelzwuqdq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggeqnibtb.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gviimgimh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gllojctic.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gdbiclngk.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gadppkaft.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gfnnabsth.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/ghrpcybcz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gukecqyxs.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gfjshywhf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gnribycwt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkytarkcx.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gdmsxzybf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzbsfkpep.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gssrrjaeu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/goorvbfsq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gqfxjpxov.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gkjwgtgwo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gktztehbh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gzuzmwwzj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gzmthohmu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gymcgrceg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/ggyqgqepx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gcdhizrar.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gwguwftkm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gaafgsejr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnzssrnyb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/glbjpceze.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmovhlwtk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gjwcrlqfv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gfuoggira.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ghnxyzrml.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gbghvdkxh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gpitjkugv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghcfmwyls.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ggtcfgmrv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gmdoeggnw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghacekusx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gelpqbjuq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gwynxvwkl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/giyixktpd.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gbeqtpypr.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gbetnbgry.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/ghdieghrx.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gnnzwdzqa.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gluwcwqde.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvpvmdioo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gqbvisvui.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gjvckfxkf.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gnmepgznf.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gicbdmtpo.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/grotwzcpj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gxjibifjj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gogqzgbhk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gmlqslzrp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gyovbvpxw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjdgwmcc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gakdayvpt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gebyiqgpw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gbldrmuxp.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gxiqdwzuy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gxxecdvrc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gxcnzjjfv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzwckwrkx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gggkhatqx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gjhvrydml.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gqfjueypp.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gyvpmhdpv.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gnujcwnbw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/geoeroasp.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gkrubaoag.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gioobdkfs.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/grvugbgzm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gbkujveem.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gjuuuqezg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gkdmjxwkk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gsodsyrvx.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gpmqntggc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/ggztpphqv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gesavadgi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gpdbchqax.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gxnwfnxfl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gjaargpdr.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gorocqpin.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gjknpgqoa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gsfkqdcmd.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gzqqgrivr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gazggbefh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gbzcsjkvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gtipcsvat.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gmeemguzy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/govikmxds.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gbvtlvozt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gbmvmwtgm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/glxhyahtd.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gyposhkak.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/glxxgcfyx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gstrwosfs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gjijvboor.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/ghzkrakoi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gnyndaqea.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gaxgdbjcs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gprejncpe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvedselru.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gowsoxdnb.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/govlaibmx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxfhjkqev.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gejnpllza.sHtML


<!-- 参考信息 -->