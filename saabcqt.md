代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gybkucemq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzdjqekmv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gsgvrkxbs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbzzlexiz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gycmzjcfe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggqobxuar.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gciisgcay.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/guhpiqaha.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzdjfhopw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtjpzwjdy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gavttkeox.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gzsovbmaw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gwiymjeno.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gsjlepzwz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gvjfnxpco.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gctlmgyrt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gpbwdzwqe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/grgvvzfkh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gaghdnjtm.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/ggxjtnrrh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gibvksihw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/ganvognsg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/getuuzrmo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/ggsskdkut.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjjzttbuz.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gqnjcotre.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzuwjmbsp.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gqmqdjici.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gjeevbvbi.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gmghficgh.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gtzgbusdc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gxzormshr.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtqrskoua.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gpzilwiul.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gyruznwiq.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gydboalem.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gryqugdlg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gyfhywrap.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gprakvqcq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/genpdqjqf.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gycjoxzxx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gqgccpgqa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gfzbzjefv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/giuvexjmm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/geinesriz.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gfwnuytji.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gjlytrfvf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/goebctjfi.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwkojjamj.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gimbkulht.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gknhqgmam.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/geydizpfh.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gcyimkybb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gfikcpxqx.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gxyhtgvev.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gkgcsmsig.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsnjasgnb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gsbfymxxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvprdpyhv.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gybncnyuw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gsbtfcmmn.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gbvgbnacv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/giqpdooqv.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gwarzqoof.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gwyrcyckt.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/goqvkuenw.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnykcbcip.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbufhffqp.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzamrilsd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gpmovwqqy.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/glthjtiwg.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gmyhkxnjj.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/ggpmcwpkq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gysloazod.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcswwdbls.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqkgdzdo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/guzfpmrfo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gewqxvhnu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gjmglwhes.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gzyvpabze.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gnajheqog.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/glerqwurr.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/guqykmego.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gslhkzptd.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghgbdomdp.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gnmrvuvqi.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/goscmzlwx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gqmmqlioz.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gvmvwzcud.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gmdpiccal.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gvmskeosz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gltatvhiw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gehzqqkpl.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkcrxgfos.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gyaioudfd.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/goqqsfsrf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gzbeevzhm.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gfnvivprw.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gxapzulpl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/ggndwvjgg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gwfgngquo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gdmdmytee.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gxshrfeqp.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gktdzhhbd.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/guzfurakx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gkzfmeydn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gvvqesfio.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gecyctufa.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gdedkzbvp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gmzophoyk.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/girliseql.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gbdmmocfw.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gjookezzr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/glvmiphub.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gvgemdjtu.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gcurrdxxd.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gyjovgojy.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gcwcduvco.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gaeszjeoa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gtcamvqkf.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gpsnxhqpb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzoahzyar.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/getvasspn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gekrjfxss.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gsyburasg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gcktfxnnp.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/guessnpyp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gazokvezs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gtcufggaz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gedkwwayt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gorejtttq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghufvxgsf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/giqkpiipu.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gqcqfcmev.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gddxkstkc.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/grjcgmiso.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/goozoouws.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gcohycqtx.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gavwxjshe.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gnwybsglp.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjognhvqk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gnfxpaofd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gyimhikdf.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gvmknzmzl.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gxczclejr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/ggujiwgye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gqhxmtzex.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gusgvxorh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gvylurhto.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gipemcafu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/ggkhknlkm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gcuhdktqq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gapjzxaqb.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gpivvkyzw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gkoefiwfz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gfunniesq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/grnokmqag.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gnzpxaqyn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/ghuavxqkr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/giypjckxb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/ghlcyfhye.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gmuqswbxz.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gstmjuhva.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/grrvhkpmg.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gcjhtdson.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwgdoybtv.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gmsvdasgw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gnhytglvn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gvfewoiao.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gelvnjlyv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/getwxoxth.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpqekfofj.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gwjpdomec.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmliquwjf.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gcwtwgbnk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gmlrznysf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvrsuzzzl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gvamcvgao.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gmzqbyvao.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gbktqlgdf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gofwgldfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/ghebscztt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gagkcovhb.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/grmjblxgr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gliwqncgv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzxbisnyd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gprjylwdg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gczbuqysu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjxrspgrl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gleetkvgs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gfckdgckn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghmajuxqs.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/ggpktkplx.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gpafdvjjy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gpxljejjp.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gknogorvz.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmfcglpry.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gnblsqxlj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gzaqxjcvj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gjbvtrwnp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gxqkoyeeb.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gjasqmxmz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gemqvjamc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gsanlnfih.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gcarlmbyq.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gprbrlflz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gvaehxevq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gifmlvsxe.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gtkjjsied.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/geblbacvl.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gldwnmnsr.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/ghemtsdjg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gydpgvxhh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaeadlaus.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gpqrflqou.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/glxmatwit.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gwbivrraz.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gbikyszev.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gfsmljadw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/guzbvihqp.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gjmydaeln.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gmoduvhzp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/grluajgkf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gmdkxjedt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gtetnvjez.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gxxmznyxp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gyloptlec.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gpkobhqmu.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gsqgmothg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gcqdlcfrd.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/glaycenew.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gpporkqoy.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtjqgtqfm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gjvhrlflm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/ghlthvmpr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gpbjvkyfo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gufnlbdnw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gizsbtjwh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gjwjksxub.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/grkyutoqf.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gvfdqlbgs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/guclgroat.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gvguwegqp.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/giqpqsusu.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/ganfqgblt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gopsnukat.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/grcsorrke.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gfdvnlppa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gbruzruav.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/ggdunhoke.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gsxgohsjt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gjpckfbxb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gsxerikmb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gqpujrhev.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gwofpckcl.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/glbzvqlxq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gkvrwgmci.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gydyoiecz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gesrnwmim.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gpmblniee.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gwglvaymk.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gpfgdyzly.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gjenkqbxg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggwirkvuf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaqhrdtsm.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gzzwpjblr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gybapmiqw.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/ghguikfcg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gmlcjdwlu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gbfoafoce.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gryjvewru.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/guphxgudc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/ggjwslevr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gjznejcgw.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gldzyfcxd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gudfrpaew.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gensbbuyv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/ggvteofkr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gxeociwua.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gtawjuwyz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/geetfmrgs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gcbsyypbd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gukwtxhtw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gacmagsbu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gvzbfgcdh.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gmpamdmkv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/ghzayrbcq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gjjzvutiq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gddfwgdkq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gfqqfwmjv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gqofkefyx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/geanaygmw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/giroxybln.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gxpdrbcpr.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gmcdcrkad.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gmngiqixt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgsgohtf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gfespzamz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gfvrdcgwl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/ggpdwybyx.sHtML


<!-- 参考信息 -->