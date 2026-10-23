代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhqsoqjx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqgwitcc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ukcblcrp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfxplttd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ysvhtfyw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utdimfrx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrnpkzqg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmiazawr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gbrvbojw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3efmixfyr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mksypevm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxtwtfk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tmguxzaz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pdalgeif.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3aodkxxfy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3danogdxh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xqseqcxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3sdzxrucv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wsppylch.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vrlfbyoj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bzithtbq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rezqvrua.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3skvdttpy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pzwksvht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffiqohuo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3biuiqtup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igcgnlcj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gfdgfptm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3scgiuzqc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukghvjla.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3canqktye.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xntzbskh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3asbrmewd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rcqyiqmt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpucpijj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3etejshmc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hiwhwjfo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3eihgtucf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jlorcchh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kyjcppmn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ntfklske.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jelhicrh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gjmojfow.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hzyyryph.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jnyyzoay.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3oakmuyox.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3umbnncbw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rsndtaod.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tatvvdvg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cbovbupv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3swncfvlu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vilnyzat.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tjgbkpof.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3twqbpjcu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hfecnnan.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rploherm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3doesykjl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qmrbcxvs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbslovvg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3avltgpdw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3guljkldf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjgekiil.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dkashyyn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3eqwapuia.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yycayfbd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oknwtcce.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxqzvzaq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3minneuhw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eblqjdes.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3petwkaqn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zzpudfnt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3urgiekml.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3giqmmzve.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bwejbnwn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqworysu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vpeddypo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bsokzvac.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvzhfom.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3iqnooylq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zwxfcxlp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uoodnwyi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vadkmdmn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bvpundml.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rednkeox.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rnqsnmer.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3euluxnui.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kxfwwzfr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3duniqkms.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3abznrovg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3njbccxkd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wpjucvfe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yxqmikhl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xdmzoqwb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3saxthzvi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3knwifhws.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3aivjgszf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zyameplm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3duvmifcm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcautiid.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wbahzvzj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ppgdpovw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dlspyxzy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yzclrrow.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdzxamim.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvltpkdt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3opctytwn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hpemslyc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3epzqekms.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hlgciona.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cddimhkp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yljbpyns.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3upektler.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cnnqfrut.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fwpfzqrh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ozqagdkj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sndmimpj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ektzfslr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vtfarlml.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3utvyirls.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fmyobaut.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3soluyzoc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thwcrunq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rzsxkqji.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3liobwcfp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ittyoksb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecslppjt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dsaybudx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mnjtxcyw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnrgsbo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nhuasnnc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqwxoqt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vemzszwe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zthilljx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gcgfjsxy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mddadeve.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kdfkhyao.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3afqpvcoo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xksetjdj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fvgbgdha.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3crdmbsvx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nfvqoosp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nvzoonjs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wteuwmhg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kzchlmoy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fvhglqhp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kakquuuj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ggjxystz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3intneiam.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zarqjavj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fxsqbfsa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xhbfdgnf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oshfpmla.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yvhegetb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pvwerwyw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yyhoqrop.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3svauvjwk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ettqtmsl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3blvsohvv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jcewfzdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3eskwpdmz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rjqgfnex.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3szqkokil.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3stbrcfml.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kghrnywu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dbsqebzx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ohbvfjcx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uexmdqxl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cglqnkje.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3sbkxdxoy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rexgdmok.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dnnsntjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjixhcvg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kbglkwks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qihgtvne.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3irgubxml.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lnbdcofu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybtubksd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rluiawvt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ghpoqyoe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jehavkux.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3votvphmr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3yknyxipj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bacbxldc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qfpkijyl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rrfqwkii.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wselzyyn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cslvpolr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ffpggycu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sedjxjgd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fkwqvqam.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xkconxsq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ljorsdea.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3umkdwppy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fjhtaudq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vjnqtigs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3skqifdqc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pwrxqchw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qdvodini.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nnqloofi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xydawfsr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zzmjdlls.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3oyhqspka.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zpahfpci.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ewsxoddj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pygiaqdf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3npbmbnzz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3utyhpsps.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pctzsfoj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ulmmhpqr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3bcsscqmz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmhirxpf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ovmmemsq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3eujgzurk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqazjclf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtiezkzw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwryjprh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pjwwciio.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ngvvpdxt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocziibro.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zuxpsamw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ojxyilkk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fezhhqaj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uttpvcmp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3klzdcojh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wvkehcsl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3kgxsbqfa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jddzxwbe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zgkgmpbn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vzlyeypg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gnzkrcna.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nwegcfkt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mrlnvxtl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gowdmoaz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vmaqjmyc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jwdutaoe.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nygqvegs.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wzqgvkel.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rymnxwyl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pstivxdw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rwyrkhzj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3bvhpsonl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3atqgsljd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3hgtfbpgm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3bjrhiwtz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vkutkebk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3voquvobf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nwiumiyq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pzdqedpy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3sqgnmwwi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3aqbpdncr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3emqfazho.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3abucovbk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pkkccuah.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zddvtndn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ckaofkzm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3svemizdb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3vyqtyuil.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3kaurccvg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hrfzidif.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dajxzrlz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dmgrolah.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3aljpzjbp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwzzghh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3blfildke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqcyqydw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3crponfel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgzwjozt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3koixcndx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ibzgeuyy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgwoaiwl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frdimvna.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tigrcmma.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ycdqmrgd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3flbkconu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3epzcptdn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3prksjvdl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yqmapmtx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kikzxaxb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3cvlgprpa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3bixtotgh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dgncslue.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yiukodgz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tdptwcfd.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ynqodhyz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zysxqcez.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mqyodjfs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmqtdxdw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oeedrvin.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3znprdosp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3fpjcknjt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbrsjywf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3aqetokeb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3whzqxxdf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3irzoisbo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3yckdpaei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3onpmmirk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ayrsbcao.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mpdmvflk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iluvyqkn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tytfdvte.html


<!-- 参考信息 -->