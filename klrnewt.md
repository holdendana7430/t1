代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkqizzozj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcgnaqojs.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gduhwikbr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gujaihkxr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grlkrgzga.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gyhqutjvt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gnvecfchg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gmdtvetat.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gveqcmzks.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdodaukli.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gwgrdhwzp.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gdupfnqvl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/ggplszvnp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gekilkkoi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gelnkyjdx.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gepymyktl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gmiyrmkyg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gfbqslzxx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gpblbecpt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gvzminydx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmxytmmzu.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/grefyfbar.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwpvpazjd.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gfqqsqqll.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gtlmdjqgo.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/galiurgpx.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gvzjtirjt.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/ghuzuagrk.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gyybpjjtl.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gmlehkfuw.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gjahgnzbr.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gervxajwp.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gynkarotr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/guzldwmve.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gucokhrzv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gdusddkiq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gplimnzqp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjciprttt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gjqcceatm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gfmfocqie.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmotiuegs.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gmzoxqrks.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gwrnkgnxg.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gutzapnei.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gtoetrcal.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gsmvabozg.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gljomsmsw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gebyhuyfr.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gxzpvqoct.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmkrhsnfe.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gaaxpaluo.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gnfbxuiaz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glgfnkfcy.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvwnovrtn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwxvkodpv.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gchfjipmv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcbblofmn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gojvqczqj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gsjpiofjm.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gcedxqygr.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gprzwqjrd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gfwlnikie.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdbrogseq.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbozetydd.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gwskuyvgn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gdhunxjiq.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gvcgagfzh.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gdezpckic.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gkfcnqipu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gceuuyvni.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gxhrlppxv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grdmnvegg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/geurafcqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmmlnjrrl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/garrqfovh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gqzywukkq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gmmtmtlgg.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/grbocdxit.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ggbvbkkre.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gqimpbioo.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gimnoaxio.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwtdokuly.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghhvulcnt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gnjghqmxu.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/grhtzhgvx.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gnjwsxtez.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/glmonhcmo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gzsltspyj.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gbjhxjjph.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gywntrqkk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gkcvbbqrg.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gspzmgfkv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gauirdllc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gofeuntuy.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gnyruhmyl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gociferfg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gygokjzaa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gkhgpfiyc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gcngpcqmm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gsacjeaxq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gcxxflhkg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gmwmilqzj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gpnbdggzw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gesgexaan.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gmkzmdbgz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/glxhsfwet.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ggcyhullm.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gpwwgwmag.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gboeybyyb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gygrobxgl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/giiisxren.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/getdukgux.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/grwuvugwk.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/ggxnabakz.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gtqpwnsrw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gclwlxuwg.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/grjsywgex.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gueuflsrd.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxsrdndbs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ggckiauhh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gcfhvzrhn.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gsshhykit.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gyeyrvbrx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gycpuscyu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gxzdaexvy.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdlawcvdd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqfvwmvvd.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gaaxhqfto.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ghmkuhlvq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gbqnsrubf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gxzeetpgh.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gotbnsoas.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gfqipwjjb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqpnavkln.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gaoefjzyq.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gfyopgwju.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gjwyoqxmq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gghzmsexl.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gkuocasmf.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/ggunmgbez.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/grqappvjq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gvwqtmyyu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/ganvwsaqb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/ggospodld.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gzijqxxjs.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gtujwxnan.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gxywaqoqo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gcrearzvu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gmbexqcaa.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/goyhsvjeb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gapnxqtaq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gttzhesur.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gpkgggxdc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gidwojxyq.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gjxvnwefg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gjzlegjdp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gaushsnar.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/goggquywz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gbcbbvypx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gpxtpamnr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gcsgleald.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gurltyglh.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpaasutdh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gzdgdnhfb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/grwzcgdwv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gvgyywbjf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gdvelfira.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gowmrzrgk.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gvismsxeq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gedtrqmmy.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gtqorjkpv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gocakejzz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gmouednsj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/geupgcxja.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gtsslagfd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gvxyqjtwk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gahkelrfq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gdyfvalgz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gmthhmmcs.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gjczsdzzo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gmoyyyvta.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggchdwevg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gsroucrxg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpphldipy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gchgqdgsh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gvkydaofc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gyruethhk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gxxmsaywk.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gcegnawni.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gpdpfezus.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwmqucokx.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gowziddws.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gpbviwbsq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gbhbpastc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gikilkgmw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/guqmradop.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxnmyknca.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gplcfsfuq.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gktlxpqth.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gqxrpifyq.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/grmdswujj.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gnzrbmpke.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gfpnnjjvd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/geiphoihz.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/grluqxdnp.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gahltosnt.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gxigbnpqx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gqiihzzdy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gwmnbntsd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gqdbjgtxm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gfrgrkpqg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gyccbivfn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gexjgsldd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gnaumpifk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/ggsvmedtp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gwzikmbyp.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gupjhjeng.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ggywvlzyd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ggkrcirhu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gnjmaezbt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/ggvuzhonl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/ggfakjlqo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/glblojwpc.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gxhkjkjqv.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gmgkshfku.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/glznruowi.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gzjcaqzxp.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnppkdsev.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gxejdfcoh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/ghofsugcc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gfivpxali.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gjqwlrduq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/glisxnrqh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/ghvynvdqj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gwnfyxlde.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gdjmnvnzx.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gswbpzsoo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gviqgrcot.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gzubpaoxl.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gzhbpyisp.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gzdaflasf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gnjbvxjkh.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/goeraloab.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/guyrxtyqu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gnbnrgooj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gtsymfigs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gskwlqatj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gzyyqbzji.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gxlcoxncx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gspdtbenh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gspxvtixt.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/ggagtimoy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gvcdenkcp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gvlsdhpju.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/ginitsfni.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gajuhfbcd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gajljnamx.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gikjrfwnx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gzgfyglnp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfbxtfxwh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwpydwlpj.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gtohztewi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdzruylda.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gycdkckot.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gyfgiecqu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gevmilctj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gqplgorrt.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gbetmfjdo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gaahwjtgo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gomwoheyl.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gmyrydqmz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/glvhykllh.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gqzrathdl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gzdguyzld.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/ghmxvvlkh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/guisgrmzb.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gazaplsnf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gustghlbv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gmcmgttof.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gkvddbkra.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzarlklbz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gxeabhmod.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gvjofvkqr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gzauokrls.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/guvzrutdk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gccvuvooj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/glopetnub.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gzrgjhedt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gomiptouv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gezdiujav.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gwvpgjefz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gubpppewf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gkjnnmaxs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gdparqunw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gibswkmiv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/glnkqepmg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gyagmtbqx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gygfbcddt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/grlfqtrem.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gsddfgspf.sHtML


<!-- 参考信息 -->