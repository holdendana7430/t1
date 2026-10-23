代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kwcrzyed.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jcgatfij.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3twkgybta.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ajczzjix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tklgvmbb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gwhrglae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drijtetv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nhesuphy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3icvxrgyy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gynwboya.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxhypznd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bdvbcqzo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwwhsikj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nbmydjki.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ctnxcqlj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3haubhtfc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnzyxgha.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zhiomohn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zocweivi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wblhnknb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmqixyhe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3avcprecl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3flypvjpt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfedmrlt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwvxxoiw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jdfvnmkr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ozmkplti.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hxfgtjzu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bqaoxcdk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dgemhwne.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vnenpfvg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rmdmimss.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sjmmluvd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xcutrdyi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mdzzfnzi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cblvannc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rosytthm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fuhmrzwm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kehaujmh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dsaxrbik.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3afibtbtp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3trzpnjgi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jsfqeacs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xfpnkdtk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nlqtgjgd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcofycyh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjmfvqbq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxgbfnbw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pfelcpwz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wibkvysk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3daplvmfa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmeipcvo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kfctyfgf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3iqnyzkzk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdeykjik.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3expyysdx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqfxbefk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsdbpjna.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xolvurvt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxrsecoe.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zovbsjhw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gjztmcla.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hvdphbeg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ewbsrfsu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wrheevon.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mynbpgda.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gdsvkhku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vhnllisq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jpwmkouz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kffqsgym.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vtzwkjhm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cjpbhusg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvrilnat.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3syhkplps.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ogwqjwsk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kotzczro.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wnvciqpf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsxyvlfv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nfjnicuy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qnfmgpve.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dlumouoy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgejdtgu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ozmwcapm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jpgowvpo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyqjlbrc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jtmnzsok.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rotcnyjx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3evdpqikn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3npchqycn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ugsvyxcm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zvfnhadq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ayrdisxn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xpksurpx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fyipkdnf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gtudzytv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nioydmxu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dtevsudd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3smoizapt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fbzzvbvi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fizdpsab.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyfwtzau.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zvhzfxmd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytggdqzf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lqbuxdey.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xvazgwbg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3latfvwfu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mllwplpc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mtjsbsfc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3momqamrd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gerfhqxg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jgznsowt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3izskfieo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xljsinyz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fuerqlpg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nkzjaxjq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vwqdseig.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gcvlmsyy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sevqvygu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kmgzlkxo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cmbxdnwd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hgifzwxk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ekbxassf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gcunolnr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3duxtlurr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xeaoexzv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vjhjokba.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jjvhignk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gperodht.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3klsfbipv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jokrlmzy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3osiybhtv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3eippitgc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kjockjpj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3npzrhuxp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjcgcpcm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tihwwayi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jeykfjqz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uuzrozco.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zqxpixlb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3akhzgdcy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bjyrowai.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yimfkgjy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rngvgtfv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vdrosmvj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fgabqnlm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppmwvfna.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3klghzbeq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lzoeexfs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rzaipjty.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ajokgxub.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3koggcwdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dihzfzwe.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mnvolpdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmlsaqvq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rsggghnm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ruackbby.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vfcxrpbt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bblfnjoc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hokmjguo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxbxdoea.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3axlfdrxb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfeyppnj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3oqepxfji.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nmeffxvm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3sdbizvnc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iilktdzk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mrwtlqru.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tqxcqwzn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3khuxnjnv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zyzclzxu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayertvtv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hwkxevbw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3awvaeyqa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yaeibghe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fquqtwif.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pkmqokos.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fzqfjvxt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3suepvuhq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3sjlqyrhu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3cqbfxmzl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bnkjyxim.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vybvzlnc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xymqsjrn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xumkhumt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pewzrjcm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3garnruud.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3odiikisr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3smvmrbjs.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3oyhaefgx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cphpibur.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3adhyflok.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mgfoajhq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynefgsfl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ienqwtpb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjkpztze.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljvspndg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxajoll.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3wgvewknd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3exzusvav.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dophdjyn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3iacsofqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xbqeisbm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3letzsdru.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qsdbwjen.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3eaupollq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zkrtpwsj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtqfysp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gpvgqrzn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3byaqxyno.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3chgqmxsb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xpurqjnu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ixbyvwdg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tibnwzth.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3cvagwzme.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lfmkgbji.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pvzxoted.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ktunfsvn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3depkvyjz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hgmqrwxj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zkqxzefi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3opjgjujf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dxztfpap.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xybiwcfh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fzepcmrr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3eedrdjwg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xlarzxno.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3dwrdycnn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gacrzumb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wyeocrvy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rxjkwmwj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3htsicork.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwbayee.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ffnhzozl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3crifienx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fskkbblc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vszuiadj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3eibmguqh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ndokqsix.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mduwqnsx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hnmjednr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xpopylwa.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3okpeufut.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbhvhqu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3anqpnhyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzdrlkjn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3cdmhlzst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ziytqzpi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lxnxkedk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wbxxhqfo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uloudvlg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kwiyzirp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3sctnyyep.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xpxbjbnf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihcbmpvt.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mefceitr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qcsxvzao.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ckchfmbj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vgehswhb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ujitppjb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3clynelmx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3udnbthvp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3cuvgbosb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3miuhemwo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zmwnoael.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjjuclqr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3loqzggap.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwlaolvx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3auznozey.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3mhgkzfae.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zomsutmk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tfajxqmd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3itunqpgd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cmxwptqs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3umkxudxx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jyumoohg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dnxbnzwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ybtghqeu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pfrrzubn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3wgtvbnhm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ysawhyzp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tpxbxltw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3malcuftl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gwagtgdo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ntgzapof.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3mzvxqjjl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xikmefss.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qfjjddfn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3sfepvhex.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hgizfhrq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fphuryls.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zxltxdgw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3uvpadrhr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3bwfuinor.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uipthyym.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ijlditke.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ezpfghow.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3epwwgvrw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uocshtya.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3aekjuuxr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xcsxuabr.html


<!-- 参考信息 -->