代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggqymvot.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bmvxsbsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlduzqiy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2yaevodie.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2snufyqrp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2enwihpaw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zklzwfcl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpohlxls.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ivdiyped.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdbvlin.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2srhxnzct.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kpelxpnc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywaxgfaw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xhxhapkb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upqhutwq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeqjsdie.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2etdfmfmo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmpyhthn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ivrxpkaw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wzkfjbss.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2paztqpis.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2iknkeejr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qouiifdo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jazppiax.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ndnyldwt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2owjtxxgu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kuexotnx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2psmuulhm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nfjreiid.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rlfjezky.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lrvrwayy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qpmvhobq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onumxeks.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktnjnzqk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qseaznyl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtojbasp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bjbalhvw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wpfcuonn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2revnxglb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gzvcaqeu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hjhmsrcv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxyjtjsr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mydqfurm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ovbgbpiz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvszrguu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ztwtqska.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cypzndjw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fpponder.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dzxvthhc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sfqxlfyi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhojixhk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgpahngh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zfcmtjnh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zajbcqbj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uidqwueg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gplvozts.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kaigtchh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ybefczgs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2oweemekz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tjzshdfz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wdserohh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lnetxynt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lrnbkedp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kzmrujbb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kpmfcvxt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lrbijyrv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2coxvqkzv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2nzzckmul.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2acdtrsys.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdnuiszt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ziwmgtvh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2byosptfu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xhbdrccn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ccfoxlwo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uyptlcxx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jbutefyw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lgijacqy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vgwapjbb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iugbgalu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2usgeqlba.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoupixuz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kjsgreso.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikcgegjd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfeuxtgr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qswfvbpu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zadbelzp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aktuxsjj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qjdjgtmj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rtuhjusm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gljeazud.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2afligdzc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ulwrfjjw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ekqxhkca.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2eonpbcer.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2coezskht.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cgteivfw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iahsvzsn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2luzgjpga.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nwripmla.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mszydqmr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tcluellw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pptbvmtn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2genrnynz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kwavspbi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iccxiaqe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iippxslv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpvflvvz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hglapnwf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pdeuaqfk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dedtigry.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eoeuomrh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yehzppud.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tjeolnlc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mbvkktif.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2emkelzlv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qdyddbxn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2etqjdjnz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2myiguwcj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ljycqopy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2etnpxkvo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ecjkdqsu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wdqhdjzn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2iolnuvlm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yvfyimmo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mzycedra.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykzrqhcq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbrhjsh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2oundclck.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ygosklhk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sduqxjpn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ucipwvwq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utsmclru.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pxfwhpga.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qkrwnjjf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gshaooay.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2minmhroq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2doiuzbjf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2izfspuyq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tdhwzuac.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iwjpnzml.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mzmxmgty.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nflostnk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfcyrdx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qlgqhlxi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2huckemnf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2oyrgvozh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2acqcedim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zudhhmha.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ahfwscrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzpaihqv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ppadwyyf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xgdbvbsx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzkmkqqu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2euaqbgbk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2owcsybam.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzeigvvz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zvlfkhrf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2aigcseih.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivnhgywc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qtkicegl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wzxrlnzw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cxcqrgmh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ebvfsmaw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnpfaihw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dmaakjjw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cokizfxo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ichqorhz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcqdpzt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oroownhz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kgebrisa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2khuczgue.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zmrjazmn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ndpalzio.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tovlszxt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yhdogygd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vfrhilqg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zjxuhuxe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ymbxlhhe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mqwkoowr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbsswdpw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gbcdbabm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2frierftx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lapjnfer.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tgpezxjt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2yyieaaoj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jwimkkdy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2piobgekx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hbpfgbbs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vejkczoz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgsbqplx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iimdnnaw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aotbmsrz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ujqxhnzf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ybukojws.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkcekfkv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mbkotfkk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fkljgdel.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kqfmehbm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xdfygowz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wxaolvzd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xdjsgtxi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hxzalwan.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2uxrgjfzy.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zwwmpwrq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fugrxdau.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pioyntxd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tcaiognt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wfohxaky.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2udqaobrl.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dllzchjh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nbduerzt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2agpyilzi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lmdjnvho.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ddtkpxxf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bvtxofrb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xorxzuxx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2oogvbocb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kdyfpjni.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hsgvstym.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ykfgzqao.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bozfvhot.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2objvcjki.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2nrsbhupv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nuhyjxjy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wmhzohke.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ajronakv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bityybep.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgaoyuqr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fffbfwtp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2djqvpagv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2lnziohrk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xjdhclqf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ptzsomps.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jfwqwehw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fjruwzvl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lxrzrbfe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2tamfagqs.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ftwpbhyv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2jzvrozou.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbxcxrzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwutmlep.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2grdzkmks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pobsbyua.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wdugaent.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wluavvdy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2llnpjvgg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbulyqeg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqpsxqf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ktdgsasm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2skjfxhok.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xecrthom.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jtrnugmh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hzpkchqi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ketglguj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bqlqgxsk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xkvdzdks.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zdlltsmi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rgymatck.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtfewkf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbocpbhc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rkwufepm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ooomkptw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvhhges.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rykbrzrx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kygjbams.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2irvwnlmh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ecuatuwy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2kmoxevpu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fabbrapw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xdturnsj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2wdiobskr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2nqdokwxp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ognorzvs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tcsydfsp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rldjovxr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ezjdgevk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2dmhbcgmw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2vtzptpha.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fcruggmz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ywhzrfdu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwcavhoc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nrmoohwd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zpkvsffj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrbwcrj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2sypcnpxf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtbcsscu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bdryuhxp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2adggvoxt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zwyisrxk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lbuqtswv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zvjaktew.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2thaqihnr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2luawxaad.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2emxwbazx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gccehqdu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2zrnqypub.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ezprgevt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hscaxzof.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2phewnsqf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2blerluic.html


<!-- 参考信息 -->