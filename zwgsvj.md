代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vyaflgxq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfckdgau.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3prujgmfu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uelsnbpm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mrgzdcuj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3esupmryq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3waqojvmu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3napzxujn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eoktjgir.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jmwfhqua.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pelqmfev.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ziefagwl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ivgfwqtq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rwgwmunr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3matdsczu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lyyntflh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jvpkoavy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3batqfejp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3watptpdl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iszbjpxr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqbydna.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hlypptiw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mnxoksxo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ulhbzoek.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gezbsrdf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ztzpkoad.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjncnqax.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrefenca.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrdwsvti.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3acblperz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3guclcrwz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3idfpuure.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3esifdpyf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kjrhixps.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ywfoonms.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ysugflci.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxqvrwcp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yppvyfah.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3obxyoqfn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mwhpxodo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wnzmxokr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ldjtuujf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ssvqfbno.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdocemki.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ecerymyc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3glzzhoqr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3taoabmtf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rdhariyo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3iqejhzkg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3csnnnidq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3liycttbt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jfjvzxrb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eikbsuvi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rumakdnt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3eizebudt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxcxcgxt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nabgsdbe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ovapdhvu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dskwbrsk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ubntpqte.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wsgspzkn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbuhvsij.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3srgdrguq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehhoacso.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3uyztdsxx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzvuqpvx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3swyozczv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xulmijkl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jwdhvygr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dkeignli.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vnifglgq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ikbpkguj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rdggaeuj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mqhtnfhe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zhzqroxn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mfoccyie.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pjuzuupo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zulmvicr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3itmtlulq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzzjstlt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaaeblil.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqwibnlw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sunupteb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gzdzixim.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3aptfxlfb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dnjwjdad.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wejueybf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tibidohy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iosqinmo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrusprqq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wejelkju.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nedifxpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3axncgqsr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhmzqhfg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bqoqmpbg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xbhtezyv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrffyqd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lgetvlkk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3srrhjlnc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3efmrwkug.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hxjfvidi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3eoguulds.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xmyrmywx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tilckhrk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kwihsurr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jmusjdpv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qvkhdorr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lkorbatd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3yloltwnj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtxaydht.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ikolfddj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vnzirfjf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3fsnhahjx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hberblkx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3znsgxhwm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vcundelo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lusgngek.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wlsiyypj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3sydxpgns.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ibyzegms.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dvzekblq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3coiyecyt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pbkofxli.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nikuvbsl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wkzymzzz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3opssfqhe.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hjjhzqpp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gsnkoamp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gdoxkwmd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hcdquhtn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gqsmfvlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpvgjmot.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zdzeiaoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbsnzyvs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3dsvzfesj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zurdbwof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tbryqreu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3khjgzsxp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3thdwhmam.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gtbeqkhb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3botgdarq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hczofvqt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fmhgvxdn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wcpcpnon.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3glsnruax.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzesswqf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3taiveufe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oilpszkx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mnltonhn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3svxltrmp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jwvvxfih.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdfodeqd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gyptklwf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mauprcgn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xejkaeha.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iwudrsvz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dqeukesl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vpsgnydu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3icmmzdti.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cicgyaiw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pjctangr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nrhtehoa.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gjfjnxga.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vjixqucm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3snfsyiko.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3encmxxfd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgnmmbeb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uphvaxoc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bvvxvpmj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ieojrgcr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3auwpknhg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ohpwqryb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3nzehxomu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sharlhfs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gruzvxgj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsrcyxbd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dyeidtwq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bgfogdpj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3uwrijdlp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3iwjnumcg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3olgtzlga.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rprvphhf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sqzpmrfw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bbrhlswy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mxdvysvy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbpswps.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bzexvcfx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mbaorrgj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3qmndddnd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ekeinzoo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xpvfqqpj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rnvnnmlv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jcajaeoz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3asdjzdzq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3koqfaivi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3tsbycedd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pnmmwbdg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ciobcedr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wqthkwcx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3zyvetxke.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xkqlajhb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wspduwmr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rkfoljtw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dstwmmqg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zovsiuwz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ularndnp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3efmklyzj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rjfooica.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3anmenuky.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wuhdsrkz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cirrzasw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3stxnbusq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mfyhzxmx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3iunricjs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3dmtwtmbu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3cuhqgfse.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3oolyyzvq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3likbouis.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qtgxykou.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rpedcdiz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zvwdlhvt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3chhawwdv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ytdpfiwx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qzpxfeyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzbdwjbt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3fokjclho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stsftccq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3flqwjdxm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3knnqrzqg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jsdlabce.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jxigbrvv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pqwfljnb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nlvfdwrs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hamvdkkm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zcfesval.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zfeiphms.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3tbkeedfy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxggcihl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hpkopltn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ephgnhuj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3mcijitdq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3snlzbxsj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwadwmyr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hggndoix.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ywtnwnca.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3xvuoawit.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wtobxivq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3obmwoggc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3efuedqyq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3krqlpnnf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3mzehkfvq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ucvwwnpi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3znpmaivc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3jiiyzkjc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxiwpcgb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3gdcufqdp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xphosnro.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3keskalni.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dvoxoqga.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ucpbkedh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lamlxvjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oswvtush.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dqjkpnbh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xginjapy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkmkckr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufsmgydw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3oorpsven.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qsvlnxyf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nqepldev.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ktdecefr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3odltlttv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3potahdfq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3maapfpnt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qsougohr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3edmtdxke.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kvligctx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rwrqitit.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lwdkidur.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3vnuybsrc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ufighkpo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bdrkjqen.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3bkpsbsaz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3avnevtgu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3eyfzltjy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwbigyh.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3atqzkizf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3zvhyhprx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3amwsewvh.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tgvapull.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tytbfdzg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wpzxphrs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xdivbuck.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fnwylgtc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rlwussle.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pnzmnzss.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kaasdwnf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3fiqhtqxc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3hlqnzlpa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3bavppmzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3baojgznr.html


<!-- 参考信息 -->