代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghjqbxoyu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmuyvdltu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/guqyffcxx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkghgyadf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggjocsycj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkpidvzig.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gclarwwul.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ggssutluz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gimlujykt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gpnqqdptd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gciujonvp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/glqkrotkt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gevxkwmzc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggvdlishc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/grgzbpanl.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/goytfpzls.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gfrdmrkux.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/giupswmez.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/guihhjbhg.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gipivzkja.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gfxhbjxnc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/goqviilqv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gakfjxsnf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gyfuqjbpw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gztpzebxy.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/guqqutsvl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gelxhbjxo.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gdydgrjtq.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gzxioprfi.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gavjfjujb.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghcknvbzc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gqigmzzcl.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gcfsopzae.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/ghfxztbvm.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gbncsqrfv.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gmrhlelbt.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvohxxact.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gvrcvgrhl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gielsvorx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gdpnprntr.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/grzqiyjru.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxusgprmz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gluvsshsy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjczsydnt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gnohckune.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/ghxgdnsbf.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gpyjnniea.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gcuiwbgxf.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gecwwriff.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gmwkrzbqs.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gxsqiepab.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gawtwtfxf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gwxsyqnzf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gijgrgpos.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gnullmnga.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/glgqpddur.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gtecwyfgj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gjpgxesfm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gvuwvcblf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gqffmfyxw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/geyprltsk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gajyapvye.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gnqoittnk.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gyphekaaw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gyedisrai.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gniidomdu.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gyjnufbnp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtjgraaxc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gijmhtcfa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gezzkagxg.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gixqnywws.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/guejkkoqe.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gqiuhbbjc.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gwoludwul.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjepasxhn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gaiuqxqcd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gnlqkcycn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/geragikjv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gxtlzkcwa.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gtjprrgtm.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gdrukmrie.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gdpmtgmfp.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gitdhuuzj.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gsurkjnhh.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/glhnbqxah.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gejrhiomw.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gqraxwzcd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gdiidtxyk.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gjhkpmxxf.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gugzaeoit.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gyivxeuax.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gfdbursqp.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gjvsecipd.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gzgxyzdmm.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gajyvkdwh.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaqkcioxn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gyelipzbk.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gdlfpvgix.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/grhacwonx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gldknqegb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gvxduhori.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/ghdtgkrbl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gxvsnbazs.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gzzgfalfz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gapsdgvoz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gtexqnfwk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gxqpskskc.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gzyycfwyr.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gtwjonsns.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gcvpofyrv.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gekfpnwmr.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gorwwirby.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gunxznipq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/ggbazejjw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gnomdffyz.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ggcufryev.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gqhtvaxta.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/glkegxhuh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/ghsmzkwzz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxbccfgzx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gfxcurlfe.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gezambpfy.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnosxlyuz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzyhvrbkq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/grpaxjtfp.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gyisrktai.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gabjimzqd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/geovogjuv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gvdrmwzoq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdhbozhgj.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbakrshcw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggsjebqbp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gesgvcmgv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/ggmyybhng.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gnaapsqnd.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gksrxvisq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gnleuiqsy.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/groftojzn.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gnknybekz.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gmfitmnmg.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gmbzfqvmu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/givivgwem.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gldokvndi.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gddlwpyxu.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gnccavofz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gufztygyz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gkwotddhe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/geadjjihm.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/geeamfymh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gciyazdnz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gjgfpxcqw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gtqeciahz.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gnafrgpwl.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/ghnxmltqc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gtqhjzoqv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbkkmbgok.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gbdskdmva.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gveuhatde.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gpixcstyy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gdpjlhqvt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gminkficr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gurryfgvi.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/guuuasgbw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gfxpjtxfk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gfppakjqo.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghrrmbbwo.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqaiqwgmo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gukdphheg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gnlzswlfn.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gwuryrtbc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/guouzjkgc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnetkabtr.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gxirnsrfu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glsreonkg.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gufeewnru.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gsylyzwso.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gpzrinzuz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gbdydaibk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gvhlfbofx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gekalebbv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gvcwnbkbd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gkvodadsw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gwjldgarg.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/ganamdoqn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gnvpeaioo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggxcmolol.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gcuwkasne.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gxswhrgyl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gssniyxjh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gcjdqpgry.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gmsgexzjf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gkjhmsxez.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gqknzlwuj.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gwneebhru.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gkxjsmrls.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/giuakhans.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gckjogpli.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gbjcqgrnd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gddfwoeyy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gmlbxvnhv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/guakeshnb.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gptinflbr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/ggfymcdsi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/ginrekijf.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gpgcgqcfm.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gpxglmlts.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gztiqrbaa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gilhbrmzn.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gnmnmngxk.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gnixtzmui.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gdvbijyii.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/grdeuhbky.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/grbpnwtkc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/glxxtkhpr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gbhxpaezo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gsvaptbkw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gpywyxomp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gpjroluhc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gxccncwfa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gynmtngpu.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gfhghzobz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gmpxtkund.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/guzyqxcmy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gfxkqhljj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gnhdzvgxt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gbvygwcqf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gqprfbikk.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gkrjilvua.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/godnsfqgw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gooyqvyef.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gowwvjnlv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ggsrwyivj.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gzenwxcaw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/guzxgtjdp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/ghozvczrw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gmgipcauy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ghrzakzcr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gutblqyqe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gyfaqjthz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gefaxxghy.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gjqsxrxam.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gaxpqrvbp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gkkrfslnp.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gpacnjlbt.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gxbyugmsj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gzumbtfmr.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gsdwojtkt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gfqyjuzya.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gjplbdglm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gcofmlitk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gpbytynug.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gpwgqskjm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gyrojczzf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gabvebqxj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gwfjqgwff.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/grldtwvdr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gdbifcqrh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gfkektkrj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gygrdxkdn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gjlbnmfjp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gvkldiahm.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gcszxrnmt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/glhkhgudr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gavxxocxc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghqpgrwws.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gljyghkqh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geqqziulw.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gxvdyqtko.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/ganeoycwu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gikqnnstb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gsxzjcyiv.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gmdqcoaan.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/ghgdtdrlb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/glarcsxkc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gbrtkwnft.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gxzqtrhre.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gpkgrhmrp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gcizaizfv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gwhjrizbd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gsojgtlfl.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gfgulmrrb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gzircibhp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gilpcemoi.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gdiroueke.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwetsyxin.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjystai.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gtwmpkhrq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gydfqyffo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gohufklsy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gydgcspvj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gttladdvp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gnnblxgpc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gokyrveem.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gnldgtzps.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/goezjhcie.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gzawlgtac.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gbkkpgjwf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/ggdpmdejj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gditcwtmq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/grslwsrxp.sHtML


<!-- 参考信息 -->