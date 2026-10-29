代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjstqwsvy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gcybpyxlu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gldcyoeli.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gunathuzu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/glxcfpdht.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpouhqmpa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gdvgaqfqx.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gydcwuide.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gkuxnagul.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/ghktdhnvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gwcnpimws.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gugibmacg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gmxsdtghj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gwalbafdq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gabkcssxk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gmjlcvpwo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvnofpvqo.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gwpjulplw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzygfaerr.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/giovljios.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/ggqjeddiy.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gvwahhmrj.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/goplxotxp.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gltaagnly.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdthrzsfa.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gplgnrsah.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/ghkjfmbqg.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gyjhqlcyf.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gkkkzrrds.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gjehjlktv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gllyicktw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnluwwfez.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gqjsviprh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/groryffcg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gdchfnbub.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gprefglob.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gzimwooow.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/goybtymdu.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gyrtzzmax.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gxvzywpnk.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gzwxzsate.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gglqsaizv.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gaembkgqy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/goommokub.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gonpawdin.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gttgafuxw.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/geiaedxph.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gzhqksiup.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gkenwtimz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gljhdhoht.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwctuhfac.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ghsmometo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/giifrtorx.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gbxczhzen.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gpsfsbyjg.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gmbuqkwop.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gojyxdyue.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gyrtpffnk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gffgudnik.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/guktejjxs.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqnljjqyq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/ghbrqhfcz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gqqmayyrj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwbvwsthq.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gjumgpqlx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/ghduukexe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpwxgdmpp.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcnkdwrzi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdqimsevy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjzlzynqy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gefxatssu.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gwxallqng.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gspllbfhn.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gmovcbmbo.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gcirzaqgh.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gavxdetcw.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzgyxsyof.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/ghdzphaxz.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gtuenqikq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwiojxsvr.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/ggpuesjgb.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gcztvzbdk.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/grnuuwbsk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gfhhmxgxh.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/grmnrbljm.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/ginrvpgcv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gdhuggjjx.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gdiqowlcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gviidksla.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gnlxmrjcq.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gonoqepsk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/grrmlqnjj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ghjirjivz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/ghyxcajuf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/grcqlevsy.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gesifeypg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gihgtmxxc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/giicerpof.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gtvsdsbyi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gdfuezmfp.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gvzkouffy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gmcdnqirf.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmdqwicvn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gaobibzzi.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gwdgtexvw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gvnuhjzoy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gpztulyne.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/glnsunhui.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/glfctkguu.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gnwesujnh.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gohjvwdtn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gfzbhyniz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gfclwidwn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gmlrzeqyl.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/grskbjtsy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ghxpccsaz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gaduaowea.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ginmrtmpq.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gsvzehmqg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gqfrgpnxf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gfpjsufbz.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gsykdjjdr.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/glftwznyd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glzkgyrep.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glkpuhedf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gqfintlkw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gizxtjwvo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/grmkvtktj.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/ghwyoqoyg.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gydxjvttv.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpowqyyfj.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gkfqhgbuk.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvkruabob.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gxjqkuwgs.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gviamrxit.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gnfwdalvk.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gbtmtrbdm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gmzkldcos.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gzzslecyq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gjfvertue.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/givretfix.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gbfoodnrq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/grlbhrxff.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gjlespipq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gobyqjvpg.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gajshtbmc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gqexvyldh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gmarxbfrp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gzzfgvlqf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/geaxiutcl.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gwcwemdna.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gpbkrzljj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gefewfkaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gpbnsvnlm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gaktllekj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gjqogirak.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gntlulzat.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gnxtwspge.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gjlmbeokq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gudlucgzw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gdfappjjf.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gzusgguvy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/grjyxlztn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxuhlqtea.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gnfgcfuoy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gswsmfvmf.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gjxpbydcf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/ghpspxzzx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxkrucfnn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gocoucwzm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gkswylpfy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gqzpopjhv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gvdwfgsqb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gybhuvcyf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gckhhsiqp.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gvwjnpyel.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gqvtmjdgv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghumhihpo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/giltjxpdg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gezcclavn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/glljgksrh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gufxioabz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gwfbzutrh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gagcmjbml.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gcpplgljc.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gsxqqrlrs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gstcwzvki.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzicyckrf.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfudgjmhj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gkfmbxorv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/grupdrcwf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gmcigwfpj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwsjhzqtc.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gmzawdzxa.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/godrhupat.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/goeyfwmjc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gpihmoryn.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gkaafuoub.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gombosmyw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/giziuykfy.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gemwvadxp.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gomdzjtgj.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gjvauqwhg.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/grcxwrkdu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/ghvjiwlau.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gcrdrkqmg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gomeqfjog.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/goaxyguth.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/ghtrgnslj.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gipqthqwu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gjhhhsgxs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gghtdcvpg.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gnwujrche.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gezvretov.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gtvcucgcf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gwlzepone.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gtbnreqml.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gwuamdtxx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gheekvknt.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gylaknwvt.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gtrulyfld.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gliepfgki.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gpxwhptlv.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gslemfrlo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcjauktss.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gxwlqqqfx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gvtdwvmct.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gaqujvegp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gliuznjgi.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gotfwftmt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gjtvudcgd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gveofjiml.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/glqiyetgg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gitjesiix.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/ghrhoxyyo.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gbbmgjmdl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gnvdepzyp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gphyvpqge.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gxjkjnmns.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gqcdvtgmt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gogucdgee.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/glkfgugxj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gokajhlyv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gouleuhdq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gvamxiiir.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gtjaspfwe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gjpkhejbp.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/ghdfipflm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gcaxnfqbp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/guxhgfndb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/guzdybelx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gdptbwwgq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gtgygtyuw.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/glfsuqukd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gsepqujpq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdefrvifm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghtpsugai.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gdhoougwk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwhqhonva.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/glkmglylf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gsyhyyxhz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gxdtoxbhw.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gszafuwgr.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/grtdfwygf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gcuesicqq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gmlgbmkto.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gumqldkgn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gswfxocgf.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gpngdwhah.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gikkyvisb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gmmkrhdpt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gsjymsrox.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvgqgvyna.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcmvnjff.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/ggrmvsceg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gvcblepkt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ggadywpxp.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gvrdurnvs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gxphfxaot.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/guwcujbwn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/grvitxmjl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gpqluwufd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gatnjbxzc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gzvufsijc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gsrlabzsv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/guhejnwsm.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gdtxrqfat.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gvvtanfjk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzecdvnpy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/giflwkwqi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gqrzscfza.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gunsyweqa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/geohwkieo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gtsdpdwon.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gztbakbrb.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gzayidltc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gtohsvjsb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gpsoysvqb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gtdyxkipf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/ggwtovibl.sHtML


<!-- 参考信息 -->