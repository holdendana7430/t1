代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gavhlrvhm.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/godxuhcca.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzhxnhjkp.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gurzylnuv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbngkldte.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwyaffjvx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/guymrguwd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdlbgwguu.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaxfqinxo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjdacxukt.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/glabuincr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghckwqqzw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gdbuqyobv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gbogzrvbf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gffisubnu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gqjnnenvi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gmthzzqph.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gcaumgfwl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gxwrptelv.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gfjoucoty.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gwvabrjvs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gpdxqwuqi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gwfzmkprj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gckosketo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/grkxyeknb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqsqcunar.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gazkilvou.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gtlyyuwid.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gzjeyoycd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzefpdnvz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcmcmhqmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/ggdpwntim.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gzvvvpltx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gkzicaavn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gzfqaybut.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goihvewar.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gvtvrgzgl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gtycauttu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqsdiboop.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gefxwdumq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxephinbq.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsncjhnac.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gaonhgcnd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwxvjjhwb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcbbfrnbf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gstbzzteb.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gvhafsakz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gimjteofm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gujieyzoz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdnytsfjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxgfjmxmk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/garydmvwt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gkitoitvj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gxsmkrahs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gebajzyas.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gpmskdodf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gftcoemub.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gvkrewyec.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/goqgsfyrr.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/ggetacckr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/ggqwqvcbt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gpyotkoxv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gypvjkbqp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gnfmpqiqy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfxkkhljj.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/ghybkouxj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxgykwbhy.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gchroszpo.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gbdndcmsm.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfbnvrlvj.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpmcdqoil.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gyzksoelb.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gfwowiveo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gfgxxtjez.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gnleijdlx.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gftfrfccc.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gtfyumvoc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gixgfvgup.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gitatnzlu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gcohsrymt.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gonkkjxau.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gpgolecvj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gqsxdurrx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gycvbegqf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnficjhz.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gghcywjnr.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gfmuklufd.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/grzlgxxvx.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gqesgnlef.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gpmpizrpy.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gsgusdqje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gbyvdvytp.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/govfvpmxx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gydomimvf.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/grmvgkahu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gggigownp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ggijrmfhe.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmfitywhj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gikmoysed.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gaojfedjx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gxbdnguwl.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmxgjajul.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gldrzjolk.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/guogavyka.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gpfizqeae.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcfhlskaq.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdyfgowqf.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gttwkhzgx.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gpojarcbb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/glyitbfkt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gdupnvkrv.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/geexxcpda.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/givvmifzk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/giygfybru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqqryejjf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gxgmgmhqg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gerqpgffb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gubkrpxpg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gdwfpsojl.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gpeitxxar.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gfqcrilnj.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/grnbzvqfq.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/grboawakh.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/grmmvmkux.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gabdibtxt.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjtgtozeh.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gezuhfgls.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gzlrumjiw.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/ghfzxuwbc.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ggvfngwpz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gmdnwgpba.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gjxmrgbkp.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gucynkcrk.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gkcddhioa.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/ghfgoegrj.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gwkeucwks.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gmgbokohj.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gzpcrhnsh.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gxkhhplie.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gvmhhghqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gqhsuvwcp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxthhcic.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gqtvikfbw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gasotgizm.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghaxeigtq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gknneipxy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gqrljkqhu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/glurkfqnb.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gubnvfvxm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gxrcimlyd.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gmmplmyqd.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gujtzokgw.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqtkjtl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/ggtxpjqoy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gtwepmone.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggtrjiafd.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/glyaqzeti.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gmplijeqe.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/ghpjfsskv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvasuqpiy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gntccmynu.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gvjqvfdxp.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gfedgzxqv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/giukrging.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gupgulmno.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gaavluhmy.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gbskrrjnn.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqsmgillh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvhaevozr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gghrcysdd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gffuzkxof.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gffdshkqu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gmnwfsovx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gclzyeraw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gcxdyjpuw.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gfrmdewfj.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gnnbqrohk.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gznliqxaw.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gyqrvaizt.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkhwtvgqd.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gfpsknomj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gcunhbdop.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/giwvhshzo.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gtkhentpz.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gofdtpfto.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gynrocmhb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gffurltdt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gmtacsxbm.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/geflnyepc.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/glzhxwenc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gjnpjbras.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gawdycldw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gmylcoonc.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gifhippqs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gpxkdgelo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gkebxltpi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gsrgbrhkw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsegkpcu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gouoijlca.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gpcjevips.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/glejowamq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gzotsptnk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gbchjzvpm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/guplwtirb.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gnxtcmbot.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfqoikeyt.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ggwddvdvv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gzemdkhny.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gogpktkbz.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gusgkpzdw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gqjqnvcwh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gujwvlthb.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gvwpdnkhh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsfehlmar.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gltcdrofv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/glisenbex.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gmducnytp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/geewamsrc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfenchhqw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gnyxjpxdy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gigjlnipb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gjnnzhadv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gxbvhkjva.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gjsgwymyo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gecwjohvl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ggeiwefnh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gazfaaeec.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfkmekeix.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvaseeqzu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gzsqcnhts.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gpqczkrjg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gghfdfdca.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gopaxzcxa.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/glipxlpol.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gkuuikpsp.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grdvqwgzn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ghldtsord.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gobzsudvs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gumnnmncb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/guotsocys.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gpflyggdd.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/ghaxwbmei.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gqlizswle.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gshwezsio.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gpfumvvwd.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gblsskxbh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gdnrtryly.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gzjeufwtl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gkqbpqgak.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gowblxide.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gnrgdwrqy.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gxpnzvgvh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gjwvlreib.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/givsnkwxs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gophsgqrq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gndqazmca.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gqglyhtdu.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gwhylvtky.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpjzrieub.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gwaoiyhkh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gvvqlrvvu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gqepupjxk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gwthtcbgf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gsseqnbgb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gotvlqrif.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gytiwbnrt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gzbpssgcd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gvyuhvriv.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gxqcjvlof.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/ghjnvgpyo.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gkaqhvobs.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gsqobgqdv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxnhiock.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/ggburcsgf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gstnaphhp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gudmbfhzl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdewvebim.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gsjimvmag.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gnciedxvc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/guhaetxhl.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gcvbfmsec.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/ghbxgdyry.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gyuzqoqpg.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gchwosasd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gzvdhycpz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gswjqijpy.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gnbbmkzyf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/guetjwjwe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gifvbsrvo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gebrthoar.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/ggwduzsvn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/getevzyjx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gyseilpix.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gykvxjelj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gtvmqngpe.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gbxgaymhc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gastrlddl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gytlwtzzs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/ghgijinvf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gbjhslreu.sHtML


<!-- 参考信息 -->