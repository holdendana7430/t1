代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hudbhjtw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nyerijiw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muofyvhr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvmixkip.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wxqqunxy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zetxjqfr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2izueufzj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2khbguozx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zyelupcd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zzbwnrmr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dwtpyrjj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ebpypska.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2asbmlbcq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rqdhcnoj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wwnytgdi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cwmrcxur.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lwoeaxiw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2elyitoat.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ajqcdwoe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cvbuzbyw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epgnmghp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rzqybnem.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tznvdlow.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsvhqodm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ryclaybx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zeuonfoh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2aslgjrka.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ygzcqpzt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kzqpdcro.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jmyylfcs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2polofwoq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zlalfnsr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rxrngaxb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gwyabese.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gxxkibal.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kujdtuat.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fnnqbxyv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2twoflhxs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fwrtbzan.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcktfbcb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izgzgbka.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gwskyvfo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fzkfwhfj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2knrubdmj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qokysxqk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jgpapfeh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2porufcbv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hzumxsai.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mnzibaiu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lsyjwhbn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xiavlyko.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lpdansly.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hykfyimt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mnitsnaf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bksiiotu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wlsayirl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2unbaqcsi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ezkdvfwh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tuqwguim.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynkekupx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2sxfficqq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rfowixbw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpngdpdl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tizyqacl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2agciznse.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zpskqwdl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2mdvkdwfq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjhairjc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uwbduulh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mpqexsma.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zdccspfx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2puhencio.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nbufpdoh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uklezdlu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rwawsarw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mmqshkdw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yylbvrfh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rnlwvdni.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kjuektsg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2btaslham.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2sohweckc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fjrpmldh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jihaqaqt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwodbfnr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrhnmclh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmppslqp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ddxczmnu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iriuuhll.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rpamizyw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2yplhvjud.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qwifxkmb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ljmmohjo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2chniylhn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kjmuumsi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cbqsbrjy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfajxgdz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ulutvbjk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ytldmuot.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2crwaphzs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ljkajwzc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wgmautqw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ydnqmhti.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wqfnawve.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nqbqzewq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tpkftnrl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nxdszvha.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nhodsgqk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2khgkfydm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mcttspqg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gdxsjzvo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2unylswju.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iocathwg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fontipin.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zlbyvxgh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gxhenkck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qlhdwnsy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zurxuzsf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pmjbizru.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lzlszvba.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drmkbptx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2niktcrlh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2afuhfdwn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ditmeowd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2didxrvdv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2oegceftw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ijuezceu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2moivqehc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2znnulsid.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2girobekh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pdqllvaz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2swbiisbd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2remgreke.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bzeynwbz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qjfohocw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zrgcyhmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rexdybob.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jbhftwwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twwbwxcf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jwfyvdju.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2csmwodxe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2fxuvqtpw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkripjwy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rxslwixm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsvmknwk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bqmgninh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kimbrqtv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xanmalvz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yhzflyxf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oqrjtwqy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkfshrcu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swhillbr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iittcqkq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2umgpkcbl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2eerysyyh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dmqvtdsy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hdajvgkj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sopyxjvp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kqvjvqof.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tktmyilg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mkfqwkpm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2falaymmr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lhxhcrjd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bxxnfqsc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2cbvuwqfg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ojxmpawo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pqenywwj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qofcmluo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqmvrkjy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2koxztysa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrlatzbw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjqzkdfz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2iiliqziv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2pzsvlbju.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2imnbhmta.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vbivoyic.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tmbpgphh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rbqfpwfz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gcmajuep.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qczqqiiz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxcfhyrn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2oxztnguc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2oecjfucg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zejrfkgf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mwprzyin.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2wsgsjvhi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2btpbecjm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qqjmshwf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qbgvkxwf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2yeaxwepz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2qkzhwvpa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ggmhfufg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yenmcbgb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bocxgssy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xepvsuvv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wgbgbmtm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nriqzrjs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eqqujqsu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vnfiiciv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2frhxgghj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2pmzmzeup.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mncztzte.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ynuanmjd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ncxqfqeg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pgbrokun.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2jhjpsokt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wymtkqzr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2inqgcqdm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hfhsvkcm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ckkdzwrg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cyftgeog.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2otizedgk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ekeyznjx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tzvrbdwq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2gfgcxnsw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zelvetkh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2izmahaig.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2eowdlvsd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2chkfcsmk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zxvrxaxk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qzssweej.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gafhxzxk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dvztyibu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nqpcamhk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oarbhmgu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2pinvmqxk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2bphqkkco.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2mnsswfge.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cejbvusi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elohwbvp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mansguhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gktgzwcw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2urziuenk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yccgxcdj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oepkjeee.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sgijqtxa.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hgzrplhs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2zdtrihmu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bcmuqqwf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jtwygckn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ofnrdxvm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rroqdxli.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzfhsmnd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2amgdprli.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2mmqtqjdh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2psebmmll.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2fssmampi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xalmbqkw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jpujfabb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lptndcta.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2tsoubjea.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2walocfbq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2dpfougca.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2findgiee.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nggxbofd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sruwbmaf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2dqunywgy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ntjoxlns.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vmlcrvrh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2xnejohwc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xayvdtka.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcsbgwyv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qwxyttcc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pflysczo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nqleqwcz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2edmzdjgk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ibqlqdmm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sfswmnzx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2aozdcsyh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzizqwct.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlahsaps.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2josbrbjg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zitrrahj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2sycopzrx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdulcyd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mohbqzta.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zxxorygk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ahjvxvft.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2leafjqav.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qcphdlji.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dwdgrvbk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2apfzjwle.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rkhiozcm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2plgmhitk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2qavvhffh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zqjveawe.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2nqddjkmc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2orsjpryq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2pcwnexmo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qakbrwih.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bbfudzfy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vbygyews.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2wynbolcn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2cxqloiyg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2fqbgevck.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mxhzygqx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2nougpbpu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2scfakgjw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lylugbmk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wkguaixh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bxhefard.html


<!-- 参考信息 -->