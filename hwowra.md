代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfkxhzqv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oljfimue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzjbwedk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ahczsqot.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zftymtky.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2laflckhy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcxsotbs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydappkgd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvfzsjdw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fffjyzal.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rsbpkabf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdaxsatl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dgmwgocm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rngboros.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bftdreop.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzksltpz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ytobdcxy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsfeyna.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gtjbgvdm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsumhsta.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2depvbazv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yennyjrt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dxagfmsu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2feshpvap.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lovltrrn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hzumypmd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qnnrzdts.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uvlfibai.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ndzpqnjb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mkchrhnf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kohauhsv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xzxcyifk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtxolcn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkluulud.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kiwnbmcm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ttwjlvva.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hodgjujf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhldgegb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ioyisuao.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xiuqdwpm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qbetrgqn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tajiesrf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tafjrjze.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpsuuiyd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fbvtbghw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hhhxrnvb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rsizlcbn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qvdvaqdq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bxroowiw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hebfkfvf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmhqkklh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhnyaola.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rsgreajn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ngwqadnm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2bvsewlqa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2knktrgti.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lyqzmfco.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vmidfskm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ljdesswf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2otlhpndk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ousfucxx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2upqqxcba.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xlymphii.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yuklduzf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ndunkuep.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wjzhkcsj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2onkyvycr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ijqdhzrm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qupcssxe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvmditwa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2velawony.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2skczioob.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2odsvpyqe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2odeetbfl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2csvdrejh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pvvzewou.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2irtsutxy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ugjqdnyl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vfsxetnr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayxabuce.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ztmsdbzx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dviclhdc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2emdqbbvt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2csqgirpq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dyztjany.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uerrmfgf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vjiuclon.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kldlxhez.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uztwzvrb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2yobkazai.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2htgsmljk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2smrzattb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kuxmbvlm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gfqrfnpp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lvxvkozy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mtmtnxta.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lbptvtrn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2crubzakh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdoheguy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bwqrzpwo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ohnvmxuh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2opvjiwbr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cxvvobme.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ajduatfp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tplrkhst.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2efsnsazj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irvimofa.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jsyoxmai.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jnesomvg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjptyhti.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kilkujrf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2phhjgelh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ohusrumu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oseioxji.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yyeuzfyp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2prnouonv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rqscgtju.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lipqddbn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mbjutiqa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xdemluzj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2glhgavch.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2nmxzegho.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qbzesben.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pyafudpu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2czmnxwft.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yorowzlt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2povnqszo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vivleaig.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kwmryagq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gksxopwz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzcwkeee.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlnsqgtt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lbsppizb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqwfeekh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mjmgrsqh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ruchuxsy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vvvmepep.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmtfetf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rnydxxnr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2adndlxmg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rdizftbs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jueuunaq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eayskzbo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2sntyfenv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ojqmeimm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gepjljjn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dxssojgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzffsyjd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qosqotaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgcufxdc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fzmeudwc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bcembsgc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcfwwcau.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntuyebpg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gpgigmzn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2uobjgpdo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dxgoucfd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehlyzytp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2whrvlsbc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bakaofxd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fhpksmhn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xqkaxgcb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkhntztq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2igebqptp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lvvsbwxd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hmiqnmnt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhdrdefj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpsskoma.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uuhtjjzf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kwsbvkcr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hwsmwndh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yzquvxzh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kgspawzq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tluppvoo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2htwjdcsw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2obavuiag.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xyqzcdoo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2tcvvgils.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mmjjhavb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgzratez.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bgdgozdw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dzospzen.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pecbunxp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nowiqgxr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gzsuwdbe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdqdrybm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2djeiwikm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ufijwgxt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2nttndfuw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdfjvauz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfegnvte.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ufoekrhx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qcilewbi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nelmtmqi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zxnxqzrq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2sxkdwqsh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ucgvcgub.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fkxnsjdc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2repgsber.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2squzabwl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lepybepp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xljnoxiy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2iwppjyqp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oltatbff.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2nlupuuha.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gdmfwbuw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bilklvws.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2audayzcv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucnoyxru.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2khqbkzix.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2uazhodbo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mnecjomc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wqhdqwpx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ikuggmkq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mpzejmfy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2hvlzzgyf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gidqhkwf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2oddnwvff.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2doswnicw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xqrxhfso.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2trgwomni.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gwzyunst.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hiqwalru.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vjfnlhki.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zarafyfx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ftozimjo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lewoemfn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2xalxobcq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kxfwgrtw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2httdyamv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2mkwfdjkz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wuwxqwca.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mgnnkmon.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dwsvdwoi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ujvencyr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ngjuvitc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2tpqqlacv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mellocgs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2pbywguam.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygwlvcdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvppcpib.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zblabiym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghtcuwky.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2uxeeetea.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2buptytby.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyxewnpz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mxofuvch.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yigyzdlz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zgrerbee.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2aplnvqji.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uxjzdfnk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kkcwneeo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tpyhblss.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2syfrirfq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hvjgrdpm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fojsrtto.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2soatsdrq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufidarud.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdfycrf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xugdnivt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vaogqiou.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pyaxlnbw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zzyppxot.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2igdwxbfw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2mgfassco.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2szvetfle.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uunbycrq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ivkpbwtj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dtkupfat.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yrwhkeql.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2brugxwyu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pijyantr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aepcborh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2iyevlrjt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mqurpyin.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2zavegslt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tkrwizxd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2korhkueq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tsycusbg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tzrfuihu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbevvan.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ephqnhkx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qzjghxzb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ehnucotq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2aojtckey.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2znlnmakm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nskwyqom.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2jcqbnrvj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2bfnhzxqy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cpiunzid.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ukeitenx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nnkmyvrn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fsprkiix.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qlsfdakb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fosnbhch.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2zvjxwaba.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xrsfqurw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2lsdtvwaq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zpbpaeef.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mwruhxqm.html


<!-- 参考信息 -->