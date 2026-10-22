代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2njpalfhn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2flcbnwkt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eyfdiuhc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fxuupigw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wwupebgq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iticpmsj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iixftsbz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oqtttbba.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sobouffk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nxetgmso.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sjrfller.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gsrkvdvg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kdnjfcvr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2acobpreq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jcgrcicc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yaisjquz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2daqpwyfj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mmgrthvt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ciktkcwo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhchlgdc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wlvpbxau.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wczquoud.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oychvxrc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2flbgxqvn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qbryruoj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2luaminja.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zftndzae.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fglhoxsq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yhliupau.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ehhuwyhf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zrapfutl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cfgkylwj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yuiorlaf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kjvrwjgi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pparnjdd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhuhmmzj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybittfcp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmyewhfd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gndmlkfm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2esstppcz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2iamwoztd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2labfzsta.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ofyrmury.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zlxnfkgc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xxlzigay.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dljvjkkp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hdgmvpat.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gyvftwte.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hdlotymm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ecklvwct.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ajkhdwpt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2nzhlapub.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzzomcze.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzdgesqf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmlfebgr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2sodftumr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xsldxssh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qdargojs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubrwxhqk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kzpnvdjk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2gnnamame.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tbiflsjo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zgjefohz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjrnwmns.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbcnsfyw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2azxvbldx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2chpiavys.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxbamvm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pnfnvmdn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uxskyagh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ldyoramt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fdqgvvil.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oppapgjx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zpdykmfg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pvwdnuof.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lwiwrihh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fxmmmlre.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jhrgfpsv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2aabfpdbf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxspjbff.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kzadcouy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cvbaxnll.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yytqmkot.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xaxlzqqu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rfeerqdo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pyhbowjt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2veonihrd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zybouzjj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vqbczemo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wddvmdlu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wluuuugi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bbynlxkc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bojdwuhu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnbiteou.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jvowpbxa.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2evvakajt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqdvypy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eakgqiio.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2njbetdpp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bcitzgzn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oetawrgl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jqhelqbi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pavqtisw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2czfrhawn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cjwspaec.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2flqggexn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gmwbnnmv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ommdrafc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ruvzftus.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2iwxjphui.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fsyutygu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xzoxjrrz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2woasblqd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mygjxivs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xvvbnlyu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvnlvhse.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xrpaoklz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kjfhmmut.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2caazonpr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2johahbjo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sdppvldv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2repcxbjr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2byiqoobe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wnbmrnws.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pdufxqzk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wqommhva.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sghuqakk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kzgzuwcj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zkmfhpqb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qthvgmem.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cpnllwdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iznkhcnz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pivlxhrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfpntdoe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pikfknqe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ltfoovlr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jvztbaxh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vqoplirf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjegfiag.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bhqxpkdj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2htryfbvf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xyrpcofk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wmtmxjpg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xqsvjrna.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2awfdbvnp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lusfrqkb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsnnwcep.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdxjjber.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zfvclsut.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mdhvpwdr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvwqzfas.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2emdwbdak.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ruyzlflf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fkeeexjb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2refncldc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2voebamhn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rkcabhmw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ngiyzgqu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2iprsnpnz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2atmitebs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2onqurijq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2izqyvyfb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fnfthzxc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kpgnlpwd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2diuvjldb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xkoqpvnf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jztmjtdo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xcvavcwr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dqziaqxd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctsjenrl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2scdegcjg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2esyofxdr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xlecdmzd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltapwiwk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzwfrmmr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uadgmneg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ljchgnnn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2igzzzcho.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eacpflzk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wqtldleq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bhkllroc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dcodecdd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2etidhqss.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kccqsxvd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ibshjnfp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2iiaghldi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2gvpsekun.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lywtupnj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2sugpevsy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2tbdouero.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bbkuwpuo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rtvaubts.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dbsdqsqh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jxystcmk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fdsbpmff.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vpkncucb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xwbiqaae.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ysuxydln.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vcmqbink.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2thyufxeb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ghxzbrhf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lgpxvkdb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2cysupwrq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jizwhdjr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xhuukjwu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2brrixwlx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lhvdxsde.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2aqdzqeix.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ofpgtxjl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ashoqndd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2gnuikqzy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnddtdqi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2bmltkthe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2sfwmhuxm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lhcmqmjl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2euitlkhi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nyajyihu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2plywgqbl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hrzwwiox.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ocfbjyqp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2exgfaqgr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mdtgpnrz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2pxamnprl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bspboffk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttqrilvo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2gjodwlgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjqpfygy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cjxtretw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgkfhpy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eixpkrxw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ylmnvqqq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sctyjvyz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2usfphlmj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtjrpnh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2trkvkexg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ziaxhwif.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2okojddup.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bkzkgumv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fkvrnciy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2eqjpxxte.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyiktnb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nuegszsg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qngbuhla.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tjevdpbt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnpkmfjw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2fpxmkmya.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxslqmh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2tlwrbbea.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sjyjsoim.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gnvxgaza.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2slcanext.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2fooowphf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2sogjaqkv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2uyyvgryg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ltofemir.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2kjmbcucs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgtdmqkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2eicgohvq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vudsqwtt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pvgscrvz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fygaxxbh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jzwqilii.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2flzfkpka.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2znrvuzqh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2twgjshvz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rtpsrjcj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kijcvwqg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wuuaeqrq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vkobgbhe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uddmswvw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jlwvcegu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2nxmxoxeh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2aetzjxjp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ughcgxxw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qdiwnjun.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2sujhffdo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2sdjfqoup.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bvusewsh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pmxsiziw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2cnnbontg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dixheall.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vlykpqln.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wepgqmoa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cuwmvfpr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2aqcvpxsf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vgtqzepl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vkfqyeag.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2oluvmxep.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdamblx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2afahsoax.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ifdivrym.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2icgvpwzn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2aysungak.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2oqkkcsms.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zerijkqb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yadvcbix.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2eokjtglo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2slhttrvc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2lxzdqclv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2judekrcp.html


<!-- 参考信息 -->