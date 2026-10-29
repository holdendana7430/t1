代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gnagwphtx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/ghmzcwnkm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gosuvgott.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfnmtymrk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grqrbfecg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtxfmbbnz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gmozjduqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtibrnllc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gymvgwzrs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggyvlfqda.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gogbpruou.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gozxqawkc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gzkffbtuu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnutgezmq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbllfylkl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gwkknxetq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gigqgchty.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggfsqrhtz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gfncixopf.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gsuennctb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gfoblunzz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gxmoosqxd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/glpuqppbm.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gxcymnxsq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gqzklsxel.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gzjmuiuma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/ghxuavzux.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gstzgimew.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwmgdrwed.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gitkbjrvr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdgglfbay.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/ghzfrewsw.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gyorzxbjt.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gkkleeqhu.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gycxvapkn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gcdxrieqe.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gepintxrf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/grccwvnys.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gzplzhets.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gescvsqtq.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gggqsfmzs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gifsktgsg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/glotcylpw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/goygmsgsx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gjmvtjfnd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gskozfqvm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gauonxfyr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gppbmiylo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gecghseop.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gsczqhqmw.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glziadjfz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gminpvtbc.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gfoysuuna.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glrgvcssw.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/grasxpjjy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/galpbgqng.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gmxrzsopi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gsevcohvo.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnlndsgqi.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glphiethk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gypoeojnu.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbfwkfgpp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gahdrkoxp.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gyfsxbgzw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gkshffkel.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gusuubtfe.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gggygnbck.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gmytlnsyq.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gwilvrlvx.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gqpupdobc.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gmfhakntf.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glfzoockh.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gentktvuu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/guhkbjycz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gfgxvlwvk.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gqdktsxfl.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gnajxcokq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gcvpnenye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ggcdialiq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyessknhe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxmtedxjd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/galoosvlj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gnzkjotsn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gohpenqmk.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gexlwtmsk.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gdkrldpyj.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gistpusjd.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gsuzqohcf.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gulvipqut.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/goervzcui.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gfjztwcfo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gxfhqykqe.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/grgongtnw.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gpjjeshgn.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gtjrblhbm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/genrdfnpo.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gggxhwnie.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqjepapov.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gcqrpaulb.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gkaxdywfp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/glffssdpv.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/glgogvdze.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghlxackgi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gcsiztqyv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gdccarjeg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gpwdgkynk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gktlxjcnl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gmwqkujfj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gghfomueq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqohcpgbw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gqkkqybze.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gdvtsjavu.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gqgkuorpj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gqgzryzbq.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gnwgttvzw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gwlwcdpou.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gckmjcfdu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gnkvridpn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gnzryauvs.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gynalursq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/glocawlka.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/guadaavno.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gpcaxkgwm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gqonycpjj.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gvabcjknx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gldvwnlij.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gphlsmyve.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gwvxtnjol.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gcbuombwc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gpspkybkq.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gzurkavwr.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gutmqjjvq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghuakdbhp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gbbtbeciu.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ggwgmzlye.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggtmejorp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzssoybck.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gfkaasnal.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjvgxybko.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gsjshufpt.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gmilqujcv.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/grakvraab.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzdcyoolq.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gifyrcxoi.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvjdeujje.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gdgigpmnj.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gqyypalpu.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gejljhjdj.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gwsrnuhhn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gmseumyrc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gpoerhlqp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gpxomduss.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/grdimaeeo.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/glcdbkmaa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gyreovrbe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/graqvbjru.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gdwwqsaxs.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gaevaqwmb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gbhqfnxgt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gtsbzfueb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/goinywutb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsrhvkcni.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gpdudhckc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/goylkhgyh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gxyawswgj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gnzhdmlwx.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/glbeebnzp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gqccxgtgr.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/goeleizac.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gkzteqllc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gelqaqlte.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gsnxgcihw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gbjjsonkg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/glfvzlfot.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ghlbuccuu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsmqbezxb.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gvmhtghpk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzcusoioi.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gamfiqetm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gkjukumef.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/grcsrsxnv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ghwvuwofj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gltblxvun.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gbizbykvv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gqzuozdlu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/geahlncrm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gldkpingc.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gdjayykjz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gitunvytf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gaqamvhgp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gjojpcepp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggyvtohdh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gttpoasym.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gljhzhgbi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gtyvchzld.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtzbqimuk.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gxbjjeuor.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gygtwyqdm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvunvsodw.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbrbvmjjt.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gygioqrot.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gbakiduzf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gcavfwofc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gxunfcdre.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwnnrdmdu.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/glsajbwcd.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gjwclcqwz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/ghbmjwdqp.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gkyvikjxn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gkmsrwaee.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gvqyhljdz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gssznnjug.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gkwpdpaxx.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/giyfwlgbu.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gtluxkgni.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gwzgwaayw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gaaddbfcq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/guaxufsqy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gohqlpkfz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gswospyax.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/ggfjgtlll.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gqcyrfekj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gxwmxbrte.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/ghpfnfmjk.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/glqnzicgt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gsucxtxkf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gjqdbghhg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gthduyatp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gxywcgbnz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gfvixcawq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gtyhdpojb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gfpnkzqzm.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/ghzmmcpjz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/goiodbnyv.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gkmcrzaww.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gcgrizjbw.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gaeikrntn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gyaghumml.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/grvbyhjxf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gdpoznihw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gjqryvqoj.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gyxstsznr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/geddhgyxu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gpttujpyy.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gaqoktpqn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gubssameb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gophevtlw.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gazwzdmio.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gexeqqjqh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gxmxlmqoz.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gepkqbzqa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gpwqoazvk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gxkkrvafo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gddlzsueo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gnbeqoklp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gvbxgyurb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/ggutawvrk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gsryvphpv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gluddnzlb.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gypbckgof.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gnqbknntm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gvgtrgavq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gmtkskyqd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gbwgequog.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gtqmypfbz.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gxvznuhtp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gxrxpewkv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gudtkusst.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzsjmiqlz.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gvvwrkimq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkpjhzwsp.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gbsvvvzus.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gciiyskxg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghjxnhkob.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gwmnrdmmg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/ggfqbfpzo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gyvifyelt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gdikydwwj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gbndqzdbj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/galzwkvkl.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gkkwtxlwi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gpkquokuv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gdebthdth.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/genfjjvbd.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gkmumytwm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gkrrfpkii.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gjtksjegi.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gyjxugmzj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gndoxfynd.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gphdakmqb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gcnimmdzg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gzhzpsyhg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gbiqshfik.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/groxaqtmy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gurwvpjmb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gmmlxrmwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gngvqmafm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/ghpulgznb.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gktbuoqwh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gasjvpxme.sHtML


<!-- 参考信息 -->