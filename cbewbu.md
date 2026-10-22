代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nfvusyuq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2adrnvxqa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2evdnuvxm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgwjdhip.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tsvculnv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2erkhqddl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfbctzcs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mturhkkm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2saetsqlo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2spqaxgul.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ptfvpgid.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dypqgawy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dtodwszl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mgkjrsss.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aonezhea.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ybqzfvnq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vqmgosqv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nnerzehg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lcznizdh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nziuwmiv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mmsmhrxq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ilknncoz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cfcmpajv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ejemvljz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otcqwdjj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvfljkw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2myozopce.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rdjugqyh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gppglgde.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eqhziavs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2idvdyfog.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hgznqibg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dtlmftga.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gbwpopph.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqxpkzrm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vuewqchs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pjxpwtfu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2iyplnxqm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zmihkeor.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2urjzimcv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vgthiglt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fcxqijbk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjirgokc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeqrkmld.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2djjnwfhx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mvphcudz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hbizbzlk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cdcxddxv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fdwrmsfp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ohituyzj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2olaclwfr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2icbrtjsf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iotizfse.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qfdxqquh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nrfkfiaa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hcikuaot.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2uprjivyv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kfzbdpth.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tddrbiza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qsawxwtt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ramrqltx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xquqdzew.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypowgrzj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2amdctikg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2slcgbxuu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xpvynbgq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fnnxuciu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xkjfefot.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vwxjzdal.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvaynkyq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2depuvmvp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifantdkd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbsiwarg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2eaegsnte.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2illmzwrx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2pxxzornn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ccrubclm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wmicqwbo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nxrhaetd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mdpuagtx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wuqwcchk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nxkfrxqy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hzgxgnqr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tvgxpmfv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2lhltzufw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zzbwmmzg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bqwnogkq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qhuovtqz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irtgtiem.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2waunpnwc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmprwsxo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nthkhddp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hwzruguz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zcxsmfpw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fvrffcob.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2okuitttf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jcziyhld.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ajdubrhh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pvlrkbwp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2abkcgqcp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jaqpzahc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uveekqkj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uwiwsgfb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgaayrth.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nzbtpkko.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qufgjydv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mpbavgnv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tclrzwjg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xzzmnalx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2rilbfmgk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2axouiibz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2javtsgbi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xbuamggh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cxzcbgxi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2oqwyvhkd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zotrfgin.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2eqiraegp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cayvbpev.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ywwywbfl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2eaoyuafg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2afsidppq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wuiibqgy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbqenabl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wfkyfodj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kotxrvxe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2massamux.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2uxrdyorr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zgvmzqeb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2noggcmvl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ggistpxo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qpcmhacl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2recfyovv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wxtdowof.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcyjaemk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zdqnaycq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qerysptz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ahvjydlt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2cjdeyhjz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mdaxqmmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztbstcwe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xjsiiaal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhjmxzff.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2pcoqhvdq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vmbhruji.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybnqltzc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvpxoyme.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmglonsq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wudkjjlz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zbzcgksp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmwblmau.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfhvyczt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ktigebpv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fhzlvzmf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ixjtixqm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2msquuybe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tpoxmcwl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jmlaasnp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nymxvndr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2sztrqtmu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2swfqnnvh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2utezmepp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tekodaum.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yjyhdofc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iaalklpo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mketkwwa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xcjijrcm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2kkwhdusl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2rwuqrkqo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jpnivxqf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kogkvwiq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vbnlcvpe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oqayosem.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rktsjejg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcvxjaqw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cdyxduur.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vydvikng.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2epbhufvp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jugtyisj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2omoawmdi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rjwnjzpv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahkfuzfd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfwddkmf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2skkebioh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pivzcypp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2erzwxjgr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vscmmjdx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fzevxhgb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2huokxsje.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pewwticv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nphscvuc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zenmuuuq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tyifoixe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pknlqtdi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ostuewed.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zypjvkzj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ysvxwzuw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ssrvkhln.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2dsqragvl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ngwltuvp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ccsjyuso.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gnkjcucg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2wbjdjdfh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wulyqkur.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xclafjme.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cjyoylys.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rohmnhdc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2aetwpxoc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wqpatcde.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ifwjzodu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nxtckdvz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dkhcajii.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zggnfcgq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2urkkbfkj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2prkwxwun.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2fcaeorxy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2cloutgek.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wmazrfzi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lwimhykq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vejquuvu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2mmrgkasz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mxxintra.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ecakgvas.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hmygnddb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hqqnfdiw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2khoycavw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2untxuhzr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bvcbeqzq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wggeqvre.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2pyranlmi.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2whqfurjr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2jzyyrvsh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wmhdjnbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvokclto.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qrxtxpkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clgwxmci.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2dqjksuhu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwwvhti.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ivmaiqzl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tawnddje.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrbjrkxf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2qpmgtdio.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fxmpgurp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oewpgjjk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zaklyfvt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2khcnaesn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjeaznm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2olsygado.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ienvgfmx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dalnyhcb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vktgxbbq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nagcdjes.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2klwghfav.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2upkmsrtz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ntxmfcph.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mysnemyu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vhoogfoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2cqbebwun.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fvqdklwz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fvwoyljr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2djllpuwh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hwqnzvow.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bghnhxvp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2kfuyusqk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ngngopbs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2viluevxe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vdlwhana.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fqskwdpd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eckcspqf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2kxyvizso.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mgzmbmfw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tqtjeuqo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2obbsbbhw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2knyvmdgz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nbipxbel.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2thgfhuwu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2npcfnles.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2cwiiiqqg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2osdufbko.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2khbzuemd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2vobnoqko.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2vacteqrb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2twyojhoh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2isrqfobe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mysabesn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bwutkwhr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zogwyoiy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pskffzuz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2zyerwtgx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2iqiqvpav.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2izslulrc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2sjcifrjr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2udgcfxbf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ztmiltcr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2sknswile.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2xrozwhox.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2lpuevsyw.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2avttcxca.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2psizyzyk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cigamcbb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zczjrhfz.html


<!-- 参考信息 -->