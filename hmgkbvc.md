代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxjynkguz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/geleuzaxg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gksbppgiv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/glwpvcygr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcjpkewhe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtofxjjww.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gtogeguem.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcrsjdres.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gijhfevmf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ghjrgcknc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnaopjalz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gpetbqcxj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gpxbkmneq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxkgyzspl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gssijobzw.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gbnopxbpg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gbzewmlfz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gtlswfvjv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gatzztgjo.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gjpbbkpiq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gdbjwqqux.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gtgsoglfx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gefdeaqaw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gpdisttee.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxyvjnrkb.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/ggjzgwgyg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdnzwbhip.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/glaatshlq.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gboagkoes.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gomvahvyb.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/ghlxykdfn.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gvtlxgggm.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/ghrzhyszb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gdveqzcwk.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gufoxrabx.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gpaemejzr.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gpvbyjllc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/ggymuigjy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gejcwiyjr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gvhizqjoc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gomohasde.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gghpjqvqm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gdhmefavs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gzlbqxvcy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gporplphx.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gmnqsqodt.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gatcmauny.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gvchgsyba.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gemaceamf.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gtlfmdugi.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gfwoupwiw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gbhryldqv.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/ghekprofu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gcimxldri.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/ghffvlerc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gthwpnemo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gyxwmdhom.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gfjntloro.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggrnjcuvj.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukybmgqq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grvfwfjle.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gqfhgkrfx.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/ghhtheqhu.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gnubfverq.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gqnsnxfdf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gxjphhacl.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwnabwpyu.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwvesfjom.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gpympxibr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gwofmvpiy.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gslxidkzq.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/grfyvzbta.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/giwprmvwq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gcrmscrgq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpogkdle.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbbmbhush.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gzcqkzywd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gyvfwiira.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gyjamqiai.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbpuhwnmv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gehbcbwgj.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/grwgryoag.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gglzlzdkd.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gqyvciltr.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmriswfgm.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gpwlfvwqe.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmkxpeobo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gcoojbjeq.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gzbtfrike.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gykvjjrqc.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gmpmmzgdt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gylntrzwc.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gcwjgtind.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gfcvbttnn.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/ghfyhmsjn.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gcivnvosu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gdgtarzxa.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqvhsivwi.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/grkjxewnl.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gxdopuwcs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gyqwtdtbq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gbkaxikmb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gommqpgjc.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gdhrattll.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gegodljmy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gxyhbjmmh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gxkklljiq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmolysxgt.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gelwcginf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gqwwxptnc.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gwrhjzhjo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/giorbware.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gxhpzbyla.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gpsiamqwm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gjbgcxdva.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gsssfdfuu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/grdrenyrk.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gxgvqvtkw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gwidlrbpo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyarkejlz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gtheoykac.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdznehonn.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gooiwlklh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gpyaxqeyf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gqbgwwqqt.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gahbxodnp.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gvetvwfti.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gehxjhfxx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gylzbqpbp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gsxsgxdme.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gvymrhppk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gyimpbgcy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gewvurlyv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gnarthcof.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gasoahubn.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gvapzybxz.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gxkajgpan.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfntmlnfv.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gsuwodgds.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdtrpcabs.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnjwbabrr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gssugnpyr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gkmumfpwx.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gkdcucodc.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gjghnwsby.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gepnicaha.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gkztsbspi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gpyanvuqf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/guyfjbgqs.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/geimibnbd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gaykokylg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gjuscpvyq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gcfrklulv.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/ggsetvfxl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gfviayhvw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gjjriruml.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/ghkwoksaw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gklhduhxb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/ghkltlxsk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gwxtmzvwf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gezbmnomz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gupfxslhp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/ginafjyuf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gnirxdhbo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gcoiapihz.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gugwsjdxz.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gpsaxunkh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/ggujfsfcg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gbgfsqqhu.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gllbaylwc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gbhuqsien.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvueaugfq.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwmjxfrhi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grltxslbs.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/glniesmgz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gujttlyri.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gcalosqes.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gzswatesx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gjhqvbzil.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gcgwshboc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gvaennzpe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gxfbfnqyf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/giajqgaan.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gfopbihve.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gditvbpem.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsjupzjeh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzwehqqsf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gacsnlmxm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbfhzsqya.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gfriunmnu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/glbcszlyz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grasmbjlt.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gvakmbpni.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gnwjzgyvm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gdxtyrsbs.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gymjgsevt.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmdlxzbzm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gwfzbmfgp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/guxtbpoqh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/ghykqfypc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjlacefvt.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gucpmknyl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gbkoitese.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gczlbqczn.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gkmnjvvhz.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/glmvgfoan.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gugjlhgla.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/goxfsuuae.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gkyeyvfjn.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/ghhvwrwfa.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gvoyixcrx.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/giuotrtim.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gpdhxwxxm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gadcrpigi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gaguklxsc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/glilwlgvi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/goevkvinz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gcpmrlpyg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gidiygacd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gbetudjfi.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/godojtebc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gwgqvpctl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/glueofggs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ginmhfnpq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gectnobvz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gbryefprx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gfwmlayhb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gvvhlidvx.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/ghqhyaqkv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/grainappo.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/ghywhyqnd.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/grzldahgi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gzmloaelr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gbtwsdhqt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gjpdzpeir.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gxwftzegn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gduvitihp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gkqeewmot.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gkvbtiehf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gqpuecnkz.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gxndxioyb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/geasivfqj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/ggvqvatgb.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gshdhijlg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/ggtqlosar.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gxcjdslad.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gvnotvkcb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gnfqqlsth.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gscngntxx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gmfgpfskw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/grkrssrjn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gtahwodrt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gfntukpgi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gxlwiucyu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gmiewloyl.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/ggbwopntg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gtfwixewb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gpddyqdof.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gojiuidxc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gqdlurszk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gzqmddobp.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gdftokxcx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gbsnxhpvw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/guxkatbpe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfullqxdv.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gxphctsfu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmygxlsah.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gksgzborl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/ggkmtdcep.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gbvndhehe.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gfmhrelsp.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gqwgfkkka.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gjwwnclzl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gpdfnolwa.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gantoxkyg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gkttkydus.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gawrxnizx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gopghfxea.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gikebhngh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gnjgipnto.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gjqfmfflf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gayrclnjl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gsjrzonla.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gedbrvyxv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gqbagvfjs.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gjejrwufd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gljffiohp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gnlbbqayo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmkppbpwd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gjrwsknif.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gviqktocn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gewxlaxzu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/glkfuwssc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gtzzmdvlq.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gtsniqdjb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gdwjivzel.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/ggljmlqrq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gwvvxdxjp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/glmsjscdu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gkztrlasg.sHtML


<!-- 参考信息 -->