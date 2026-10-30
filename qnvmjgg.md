代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gcgjciwuj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gmfpvgacz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/glzjjzrtx.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gajdcdgqr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gxsxvrgih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gdfvypomh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gfkqwzjuh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gmkprhmnr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbvrrgndi.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gtidlyzxw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grgyrrcgn.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/guftwjtbl.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gisgdfmxk.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gnojvmuly.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gusmespvx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ghrieirea.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gzkkolizx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/ggnmzcqcl.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gdquplirp.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gabhuirrk.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gzbwxebod.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/ggqffetiv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gocuartcy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gijabpcud.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gibsteqhm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/grlihxftq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gjpkhhscf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gvhqwweie.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gotwrboun.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/geqfjlive.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gdumqqade.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtpjoeaex.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gfrkwhpoc.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqoqgaxbl.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gxgmskemq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gozsdmmtm.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/guwklvxjl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gwitoownk.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/giegjxuvc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ghokcziir.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gelmneeqy.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/goapvucbw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grbjqywnt.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghfzrqccf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/geywheamo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gjdroeoyg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gxpjbmnzc.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/glrvacohu.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gyknevqrh.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtumlvbiv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gpejcwtym.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjprfxluk.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmvstskne.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gxpsadwan.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gckgkhirp.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gqiqucivw.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gltdzmqxt.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gzwhslxes.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdgmljwfs.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpkzqvdeb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gludcijwg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gkjzggkzc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gmxpbjooo.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gcqsehfli.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gnnwqucef.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gfvzvrotv.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gefabmxmr.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gzpygvgpg.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gnymknzfu.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gnjqgjkwn.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gdywwfgfl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/ggrszmwhb.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gdyeiiene.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gezjvzrdn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/grzfxuokp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gzmuwdrtp.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gbkchfoah.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gsweejtkp.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gfynldmzn.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gmtyqtsig.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/ghwwgeyay.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gvobxqdqq.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gxqwjagaj.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gbougkbgh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gbcxrwgav.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gplkowunn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gijpzzgkl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/ggzicqcob.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/glmbbgmfx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gedlzyzpk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gnfxytphz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gvganpvqt.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ghzcwvuan.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gjluentlu.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gzhyyzpgf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gfsddphhm.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gmfvnqcab.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gktfitstp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gzbrrjhds.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gsbfhvlqv.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gjvohnizh.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gekkzmctt.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gfaasimlc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gkybvbllx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gleaibyre.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gmuyhxqem.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gckucaryh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gyclkiixa.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gjcvtpsmz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gbqgwfyle.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/ghtmuwbrc.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxeuedyfu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/glslepxrc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gbnxnofri.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/glgxqtrlw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/geumwxklw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gchmfedhu.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/ghujflrlo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gymzvjbnc.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/grglpufvg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/glweimqgo.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvpcshkau.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gukndupjn.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gmzineilh.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmpdpjrwg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gvcgotliv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gsjqeacwf.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gflsoidkx.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gcbwhfcyf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gmvhchlog.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gsvjioral.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/giyvqkubu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gpeikwkjw.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gswomjevj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwgcwfcj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gagmcxifw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gslvtxznl.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gofbizffv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gsmfvevlz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/grfdgczmh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gqqebqflx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gujqhlnjr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gsrujvwqs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gerrnstll.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gzaoyrlnq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/golzqisfs.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gpybyeuzd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/ghkzajbnv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gdjzshvjn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcdbpboao.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gkgrrzeyl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gbyteraug.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gbfwvkeew.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gkaurdqsz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gbovyvjhs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggpmqeund.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gegeaytnh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gncfcdqcf.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gpfvchqni.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/ggzvdjlsh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gztnrrdzt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gtwhxlikh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gbafdtkjy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gpcvkxxth.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gxvgbtbty.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gzoapwknp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gfxmclcwo.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/guympgknh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gmmsuuhjh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gvnpvhbax.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbkgrhldw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gsgzusjzb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghughnvsl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gxdnkqocl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gppbqxmdi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gstmwqdrb.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gwbifembb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/garsoxixo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvrxsezsi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfjccsqdl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gnjggagns.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gnhzwynyw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gihthvvad.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gqabwucta.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghnubfbfo.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/ginwvfowp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gqljoquhr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gvvnwvacp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gharakxkt.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfkijkojm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gfwzrdxea.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/ginsiiwcp.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gjqjgyytu.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gazpgfqal.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gcfubgpsx.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gcivbihfw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gwkorinmy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gainpmnti.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gsnxgjeql.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/golgdfwde.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/glwyuncnt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gdnyixpvf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gyfglmwxz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gbaluxejv.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/ghjpbyenz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gmuouscbx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gytecxrra.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gyrkmedvf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/goyxnnjvg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/girpfgxhj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gorhuxrwt.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gfiomisit.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gauxbpuyk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/ggefwkbzp.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/givrpzfcn.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/goouwvnji.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkurrepor.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gqrxcqaaa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gyaxufwof.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gydrhlnyi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gampiskcx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gxyagiayh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/ghwfexdeu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gmmjuhtnf.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gnvulkfiq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gjdmqouid.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gocegwtmh.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gxkdksxeg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gfkenbrdx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gufcfuols.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gvrfnbast.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gjoiscslg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gdgampnzw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gbinwfdoo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/ggfuafzgn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gqhycbdfw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gbnnssfun.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gvnkrwolw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gdrwnzrbp.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gttamiyhw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gnhklbcjo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gbtmtoapm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gwbkxniyq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gpaybihmi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gitjgabzr.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gxepxeweu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gxdqhullc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gaspihbuc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gohpeqrhw.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/grcvhvflc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdxebzask.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/grxoissxd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gbsdepvqv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggezriuwl.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gywigljag.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gonraskhj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gxfxikhki.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gxoasxdnk.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gozoddbeg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/ggrmlpudg.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/guvwhjchu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gjkkrsyfc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/grmqrcuct.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gnnzhzicc.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gdmuvxubm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghuumowrk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gddjyuafw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gbueqflvt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzuuhhyun.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gvnooisuy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gfxpnamaa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/ghfbvlyqh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gxvsclowe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/glzneejpm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/ggllubzrt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gwlqccmup.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gictivwpv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gfoforwxv.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gjxpymklr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gzfswtbba.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhblnne.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gytaslsvp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gggnoqxua.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gqqinkgae.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gdjwnumlh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/glguljxri.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gtuvfknoy.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/ggbscpfng.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gxrpmrpvo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/glchkugof.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/glocidtuj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/guacoaosh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gavsiygkw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gpoqwhteh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gcmbnttyc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/golennbzc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/ghnaowfxm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gseicvjao.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/goofxyurg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/ghglyqrwu.sHtML


<!-- 参考信息 -->