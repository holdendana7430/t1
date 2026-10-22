代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ppapjojd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rbmnjrzz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2afnuetdw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oecksmqj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mlhuoxuo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqfmtoqt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rmkrkkil.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vjfuygeh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uvvhuise.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kaayuyij.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2emsowlji.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zgwglpbx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pswneuep.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qdcuiqtb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rfrrxtmm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2mhmetvtc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2elaxxctl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2grxmtwsi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cgdpdxbk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wgtjkxtn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cpsouzgo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnnsevx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fybtwzps.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydyzaygt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wzfjnnua.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kqrjxapp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ncwurzqn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hhsyaqbi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lzkuuhvs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zibmunse.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqevolxl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkngupvz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2adnvbixy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uykuoakk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bitxksda.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozlzolad.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gkzzbqok.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lqdwabmr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtixutbo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwpnipsz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqcxzav.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ltfvakgr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mnofgirz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dtrktyvp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mzlvgxxb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vhgxeeuh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ayefdsem.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sizcgbhy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gsrcaxly.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wmjmhiyk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gatvfxmc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2shzmroji.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2blusyijw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vowrsvqo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cwdumgwi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2npkiswwj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2eibbqbbx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nswgitsi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2trarnbfr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gwpmbjwi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ihbfwcjx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zzyuknvx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhavpeyz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jpnibmtt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pwjifnpo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpirkndc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2mvskluyz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjfwmdkx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwucicsg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwidfrxw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hthgafeg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsfqfmhg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2arcfzjqt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fdiovegz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sombxsvd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gfbzcpwt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nmjujtus.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2oboybnhn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ocligmrz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tugjmdrn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nxqsarfw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zdilnnnc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nmdjmdld.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2umsjbcwq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2juzzrpxm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hlcavvpf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2byhrycmw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qamfajbl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jropcywn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqodhzpm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mcocsrle.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bavergkv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cijegiij.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2buzbnxdb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqrsjmfm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nqxhlijb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qhbeegih.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2peknqmih.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wldkiiwq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2havgswlb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fswoouae.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2juhkxqfv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hqjtnama.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tlnozmet.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qtghgmpo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kzqeurbo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ilauixol.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2grycylbq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ybtzkcgt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ozryrteh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xsngbcev.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fipquxaq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2urzasgfs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yeacjnmk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nubgpdds.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lzctholt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fnroxvcq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pfcxbiiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vlnkxtcz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkqunmt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nddcnwpl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rbzaagfp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yuhgpwet.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aulyogsn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2amaqhcsl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fpgifebo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tpciweci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lysistlg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bmejesvq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fyzjiwab.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqjzzqfk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ffixnljf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ycjawtfh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ppicfrai.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tfnvqnfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbkvvqgu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qqzrijzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwnotnck.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hwepxrna.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hphduhnn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lwjiuzfu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2benlqrpn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zudcyail.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdvxavbr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2lxtbojce.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuclossj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ioapkfti.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gkmatlsl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ivlsrfre.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2onmobgll.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmbzjzgg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rfudqgnw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xovumwnz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2iopvbzbo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdfjksev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kithkrtd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ldjdlrxk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dmszccsy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tujidyky.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vzrmcflf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jysmzvbx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2njgteiwx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uwnftqff.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2etruumix.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ynvlhsvk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2xokcfuwt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bwedyzkm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcygcrae.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tuvjxdpz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqoamvnk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmwopvsg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gtvfraaz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bujkpfdw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnmqryec.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hzeiphod.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vkdwdhdt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2uvtehtrv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2prlyelvo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2awmxccuz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mpsmeqkg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2luhkpjsn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2seclzmir.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilauqgfc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2glokqeqv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2htuujdzp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bzwtpafv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cjqfbskg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2imwvcwvh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cgdzysjj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dgrdhhyi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2uoprlukv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2emuwcvps.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2amdowkmo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2tjjsghfj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2neifmibd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hxbkxyyz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jbstdxrb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2owkzyhzy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mujvhuws.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xhgeyxgy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2prbppujy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2yenjvjww.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dazkkbpw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ewrplpdw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qamquqpl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pikvrthq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2emfgostq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rfvvgmro.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2dzbmwtfn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2afvxoujl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mrecftnm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lahsjugv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zywbwetz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rtgubeyh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpiuyzzi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2umcekgax.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rsztvjoe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dqyateae.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gxhdjpjb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2mbvnkcwj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2hzyrpenk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2cpnkkirt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mtivfalb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wchxgirm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rnouukie.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2lpdbtpne.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2izzvgfjm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cojgbdkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rswyfopk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mncrcihz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smmesuqt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ufzdqiqi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbrsvfvl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2axhleedo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rgpidvaf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbbgjeff.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2esrpeooj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zofoduxw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtjnxwf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eibatdnt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2oniwbhkv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kfjaswxq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hroxckqg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pliphbdi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2pniheszy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2envdvjbi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2psxnmzwv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lzrhozns.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2elyfbnqe.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2muapzdfs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2khpgyper.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vczbmqzq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2akamrivu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vabuphsn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xamdzigh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2qmkpzott.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ckzxjkrw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dkxtsrrc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qkfnzasf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhrxoac.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fdmlvxmp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rjdeeiql.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2yukghpfm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ucnyiamr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2scrllsjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2szdelktx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bailwpli.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xapdqsei.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jbzlglqj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ftwmhqbp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vtkdpefq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2twchhzts.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2kruvzbwr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vqbbaxwq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2phjdixpv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gvovqjre.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2uqmwhorf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2waclvktn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2eyvshvwx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2oiyopatv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2flagohol.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wyferpyb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2smvawwow.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pvmwsgxj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hizctqqv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2boqbcqbq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2imurkerj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hulfagxv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2movwdkfj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2jpqdsltq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2incepfik.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bvwwkahe.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2txjedwxu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2lauvkyfn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xbzsbpgp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2dvhwwdcw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xaunogpd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hdadrjxp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2eiotxpco.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jeviogfh.html


<!-- 参考信息 -->