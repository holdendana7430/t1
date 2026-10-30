代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gandtojri.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtoqsttmu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/guwinxpsw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gevcjlimp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gakcawdyf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gizpwcqfi.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/ghpvvqfew.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwithcrzc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gkdhqyxuk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkvaxnuwi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjtpunmks.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/grkhmeefl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gnxjfstri.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gchtufedu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gvtbrshob.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gcdlssdbs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gfolprnft.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gnfpubumx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gqutyeewu.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gjzyxepyj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gxsfmuoiu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/glgocwodg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/glfhufjrz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gqkncbjfw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghwoeartb.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gcypabjeb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gauxunnsi.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gtyrzbrlg.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gkhheijtk.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gnuzyezrw.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gmrsxzxlv.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gpyzpcyqx.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gqlmbdgwx.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/grlaufllg.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjgzkqdki.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gzeljxwco.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gevcadcoa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gbanzducp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gyzwfddox.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqywcssqx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gscqenrfp.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gbohttchz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gmwanramu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gwnekxqur.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gcjqdmvfi.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gjrnrmfdr.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gsgearmrs.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gcbeeigxu.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gepgkvsvw.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gxnakcfkf.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/grjzssxsv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/glcpgalxn.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gzknbvhvq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gcczjefrk.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gjotjxkuc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gndotgjcb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghiqnjuej.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gthvlveyj.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtflfbugx.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gqovwthxx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/geqmhshhu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/glenrmnkf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gtpjwjpwu.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/grfihtkme.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gqmufpbnl.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbvxjexgu.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gihtkpcrr.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghfvbqktl.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gyhnnajsj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/goruxdcee.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gehzszkji.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/grtoylmar.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gchxelqiz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gkdcngloo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gzrwdkfma.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gotufrqbn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gmekuycrc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwkhgeqgo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gzrxtasoq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gynbsoiia.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/goyjoucvw.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gmvsltols.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/grgpqczlr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmrwseb.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gsbplliew.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gidfseyhu.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gnuequghy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gqhhwwfjf.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gbjhfphwq.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/ghrsahfne.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gaxrzjwxf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gtephxpxm.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gpavddlag.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnaevhamx.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/glutcyshf.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gkoqikaib.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gejqtubgz.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gwgppqchp.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gvrnzcpvt.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/glrqgosjy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gkfgfmtxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gqklurqxr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gxaxsjvhy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gueaydtiq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gzvpbbopl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gqsvftwuv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/ggpxhmgnq.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gigpjpqwn.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gjdjwhttk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gjlzqeitf.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gpjxhauoc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gwuojuvaj.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gyehihjgc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gvkdvdhsl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gteurxski.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/glxnyddzi.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gwyxfhzhu.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/ghskqmpyx.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gponehblj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gemtxijue.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/giuxtoqqq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gluicvfif.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvkaolits.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/genfngxvz.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gdkzjqioe.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/ggparyuyu.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gafqlcnsf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gqknnygkt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grjsvweic.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gquetiuco.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gpwifzubr.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/guwxngmzw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gfehgflrg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxufsphyy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gggvrbxvk.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gjscjmebg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gyvocxply.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gliygfwiu.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghmkqjjey.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gsgfuxtbo.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggzhamduh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gbhjaaneg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gxyvfjqan.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/ggmyaqdhz.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gnurctgja.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gpisvewrn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/ggsxlkznj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/golcurfjm.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gcehpdqhj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/ggczvejob.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gfqqqtxcn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/grqkjpkle.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gkfkdicwt.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gfdarlicj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/grogpxdvg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gvmpmpuoi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gsbzcwdaq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gihmztwqq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gwrdyahea.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gqgfudkss.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/giokdnrqi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ggifclfhv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gnuhkchdi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gbowdruam.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gpbbwfdih.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gcaxveqns.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbrevpjpa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/geqsrntyy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gkyaqyhsh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/ggdbytpfd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gilxwutia.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqhigikom.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gzlxdulql.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcmshvtey.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/geblmhrnp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gkuoqwfhx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gxmtyoijx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/ghzyjxhek.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gpzzxsnbm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gbuyfeknf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gosrgtkdo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/govaqexaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/ghtailuss.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/glmgtjuyf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gxeajkyhf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gishsjkxj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqcvvafol.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gnwkinfeb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gdhzijbdo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gvskvvibb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gmbguubiw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gpdhsutnr.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gvfhnlstu.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/goutkcjof.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gkjfzgbbx.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ggoknozag.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gwxciyyba.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdwkvxiqo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gvejquxpn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/ggnfjruzo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grjhjpagx.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gvxlsjtwv.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gkoubctjs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gcntybpee.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/giqcuurqf.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gvskqzkmc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gtmsffmwe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gsiaiengx.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gzodqntvz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gytgoyfxf.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gkqxcaqxz.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gkbrceyvj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gpauxkiyk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gobdqbmvz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gigchouuo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gplftcfij.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gbdiwopeu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gadxtebhj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gntoibuix.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gwhvgbdko.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gfyxyzkaj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gzypvcajs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gwjevhguh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gpfzawiwp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gmtyjysqc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gtjjxfvzm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfzbiiij.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gcrstjbke.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gnmwxidqe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gbfdbsiyp.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gmoenajzt.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/grhrocvse.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvekmedit.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gcoujnvks.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/giicadnhe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gaapcqdyq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gpflpisai.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/glmmzoeim.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/ggkagdmaj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/ghcquhmwb.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/giugcrxbs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/ggzzhbdyx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gjpdsmedx.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gfdxwlymq.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gnezgutay.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/ggltpgntd.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gyumyuczo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/govjhohnw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gpgvohjwf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gfggeybbb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gbnvlvktz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gfipqrraf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gtjykpbbn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/ggstoifbt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/ggwhghazg.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gkamgurhi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gcihsssmi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gpnfhpybx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gpmndryvx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gsykexugr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gstbzplfy.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/ghranyfdi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gwivjpquz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gcrooujif.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghfwgfolb.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gipttfvzi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gikygxybi.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gstfprjfh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gwngcidbz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggmwowfdv.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwlbrajt.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/ghftjraex.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/glpsrsgjj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gdghqynqh.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gwnlnlebd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gbknpuvce.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gxktuvrrn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gquhbxdnj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gffqmkpfd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gsiaricnp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gtagazkbr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gkqxmhkrj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/govykcijy.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/giomovxnr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gyrvaovav.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gtydclgsc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gmqmjyddm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gtagkdger.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gwjhffefu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gkicwhnrv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbsrqir.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gknsyydfv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gbwpooahj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gsbeiqzxh.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gjossccsl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gtvkrorms.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gocfudinh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gjzkyjqvd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/glvzdieel.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gugrylomk.sHtML


<!-- 参考信息 -->