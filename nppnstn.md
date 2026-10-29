代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gmxhborkn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gatkmtxau.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzjyjdebr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gigrvsamj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghmvlpcez.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gplcqwgqz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gssoofjsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmyblvpkz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcrbzmhew.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/ghtikselz.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glpafxgyj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxkupchwr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/getqjptbb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grttjynpe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gfbowihzl.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnxamdgve.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gveuoglnd.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gphxkqqla.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gyryiqugw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gvbpzgpzn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gvbuzmeaf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/grhymhlug.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gqnlqocsk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gjukfhyog.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gxqdcbhks.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/guoqebbap.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/grmkruket.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gufqdzmbe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/guggsknct.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/goebvbxmm.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/giovoygwv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsndwjpgb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grawqxinn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/ghkagwmso.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gtcqfwjnz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/griddjcuw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/geqsvohtx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxjnemrpe.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gsvudiumj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gpdvmfzda.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gqwjexupy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/geaoeczmb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/genmcutxk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/guajbtkyi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gxhxzhgcc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gojclelkt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grhjgahre.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyytcymxz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghzyayylh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwdyvgfkx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gwlxqwbkn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gphihtalt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzwrnrddf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grfjjzzmq.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gygrclxqn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gmagmfrtf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gizezuuvo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gixqulcox.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gzmfpjacc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/ggbgtwhhf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gfctgksws.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwmnvansa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gewbtkscv.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gujirgddt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gljvoyliv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gukndpgnx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gdumibdfw.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gxbdqshnu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gtmvjtdnm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/geqhrqsno.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gwjamdmqr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gnmwqtbel.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gadryqudu.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gddegmrex.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghltvfulw.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gdjdipoza.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gyghfjmbr.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gochmulgy.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gdztykrpy.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/glolvadyj.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/geguxxcgt.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gubxrfsos.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gqysiaoyw.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyknokuek.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/girsjfueu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/ghjuwcjnj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gyqtonffh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gdwauqwen.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gssnvfgqi.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gehifscpg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gwtqvqgcx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/grpjfyyiu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/grbkkzvtb.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/ghymuhilw.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gvlaavnez.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gpgjjwofa.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfrfkcamj.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gvldbagyn.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/guugjiooz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gwxzenmni.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gwhaxtisb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gknerdvln.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/geasitqtb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gaxcwsdfl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/geqwnymta.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvpvrvocp.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gamofgwdk.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gekjxdwax.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gyqwcspuo.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/guoqrhkgq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gqnzeeqha.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gzxjsbbyq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gvdwhczqo.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdiqwzqkh.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gibegxhzs.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsaznozbd.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gktfhozmd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/ghlgeptsh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gmbklxkls.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gkyolnljl.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gjahhgxxn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/guwgaaeaf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gruwaczvk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gyeetoejh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmciflcua.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gllzbjneb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gbryavwrh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gvnqadizv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gafcfhrnb.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gezoxmhwm.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gauaitgpw.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gfvjzfqmk.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/glanqsedc.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gwlslrqoe.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gsdlrvpso.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/ggzgesyfj.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gcqgckdjo.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gimlstzfq.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/giooflrdc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/guvxjjyeq.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/ggfuhsfdt.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gwiuejyjg.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gjoxbkoti.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/grzttwoin.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/ggruamzil.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gevwhwpce.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gxbymrjjb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gxmmowrhx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gxsktuits.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gqomkgzuj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gnhemuvjh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gxukgwbwu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gwwtornql.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gaugcjmni.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gizpdzars.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gthlyspxr.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gpoblvpyo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gyqrlwrxy.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guxiyefie.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gifebzjnn.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzjisxlvz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/grnapcmun.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gtzsyqxbj.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gkgjlwnmb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gxfiiqefe.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gkasicnsa.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gxbrvcwts.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gphvswylk.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/geqzbvxtx.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gddaymlzh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gazhgzapz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbwulanoh.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gaoynkwgz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gzmmbnedh.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gjcsskvtq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gcjdppyuf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gmjxklnns.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gqflnkbpe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmmjcozsy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjfenuzdk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ggjcooakt.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/ggvzlxbgl.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gcxohhnaq.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gxhthinhw.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gsxneffsm.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ghfmieuig.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/grorvfojs.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gekaspkiv.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gbbklkkxq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gvuxmsjzg.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gegzlksud.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/goxmtirxv.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gyvdirnqu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gvrzwwslj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/glsvhnnhx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gkjxrofnb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gnzalvhnn.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gmgajfjra.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/goyqjcvcz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gkrdqvvvd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/grvjifyjr.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gihmhnbmf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gvvzydxmy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/ghgyaweil.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gneasbnby.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtfiizcrr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gvscljevv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gasznuecz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gbwydlefz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gjigfccfq.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gwwogdcem.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gqecwsvzb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gjqrwwfan.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gwgoocgeb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjuyfvevw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gfdeaynum.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gtrgreovi.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gkowujfbd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gltrklkkg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdnpnidef.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/ggzbpesvg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkaxgwlkv.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gcsbzarwd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gnzxddrlc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/goafpbdff.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gtvdjjsfw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gyenoyhtc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/guzywmijt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gtfgjzlbh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gaiaulyug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gbbhnujnz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gsiadwbot.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gxogmijws.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gizmjriet.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grvsmdfre.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gazjttmtq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gomzposdi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gyjufrclo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gvfmgrxoj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqglzhcxu.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/ghytftnxr.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/geeawnndl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gsdbrbcir.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gdvlihbqg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxtdygxci.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjzkdwduh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gebmnblij.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gdxjvkvot.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gpgrhtied.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gelclulhq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/giqardjhy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gssobkwuw.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gfydxnhfc.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gtiocxybi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gjovxfvzm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gwdfisniu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gjpwtdhgv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkporaufl.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gqkhkwpjh.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gnkbibequ.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/ghryscowz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gdadeqbvt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gqdrfevmt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gqdhqyqnr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gvhfggpug.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gqljbwgnq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gptmxlngo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/ggzycbmhe.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gfeavuhff.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gehsjdfwq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ggofdgqsw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gzzkyyaht.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gijowpoks.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gyibnvlpt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gqoapjngn.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gllzooyhs.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gocoyjced.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gtmyckvwx.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gqcttyizs.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gykozsoof.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ghwjnizra.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gtogtpsby.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gomxophcd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/govikqtmc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glncdhthb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gchwpiayi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gpbwuknhc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/ggcykatzd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gwnyjahfz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gvfarswnl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/goppuowxo.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gpkupugzk.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gdhdvsjri.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gjkjyvemy.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gfgsxaxyw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gmpzpowom.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/grateomam.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gpwoozipm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gjylhgrwt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gfpgjpohn.sHtML


<!-- 参考信息 -->