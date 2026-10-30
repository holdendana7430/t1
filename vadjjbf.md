代发 wailian999

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdedadapg.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/genjdfaid.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvbwlnwmn.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gziexrwmi.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gvjxwmmuc.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gbijkkond.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gtocooenw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gsqocvxgw.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gkmydserp.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gfjlupory.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmqrlxjzh.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gvksurhac.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gpqvmdowm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gzmjusmwl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqoxropcj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbqszdelw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gzfazutxy.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gktjkypgy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gorfxeobp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gfibltbtg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gwpfclitr.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gesvamujf.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gshhezcbw.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/ghologqhb.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwdxjlfaj.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gutyxlqrg.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gidsoovyx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gwdbgswlx.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gfemnkoxl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxzngvykf.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/ghdojiocq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glywpcqri.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gphjopvbr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gibmolplp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gkkdetfun.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gywahsujp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gqtuotyfw.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/guimnmlpb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gvbwpamku.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gvopcjouc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gluokgklm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gftzlmtgq.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/giksvmoce.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gsukeojqp.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gacxotflc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gffrvxotq.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/ggbmjzyku.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gbwyuutnb.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gwunqmyqp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/ggokxxipe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsxoozjhp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gypoucfol.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjmdibgdd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbogpmyau.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gdyhijfav.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gqlemmqti.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gqausfpis.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/girqkcxvf.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gyaxgceaz.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gyowojkgj.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gjbgjmfmy.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gapmzehph.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gchwezyvk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gilxbsogn.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gcnwrtebr.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gasdehntm.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gcwzcmmwq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gezgmabno.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gtxwlsgdh.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gzskssrlm.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/ghpvlnjnt.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gsmkgtlqd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gcpipajpc.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gpxqlzpiz.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/ghdtdnhzo.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gkyrbejis.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/ggaekoqpl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ggftvsyrb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/glhtrrxtj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gunfsdyyw.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gdxsegfnb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gczuqmtfe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gjzsbdvai.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gqawuuwsk.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gkzjuqmuw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gvklyzfix.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gibidbhsd.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gjblimoed.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxapiucnl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/giivpyfen.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gbythlecv.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glkinjlqm.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gnypypxlu.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gphxwbcde.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ggzbkqozu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvrlqqsrp.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gjeduvoap.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzyumjrvz.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gunxxuapg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvgqwdrvz.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gmyceraqf.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gyeluxmcp.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gmmxuzzwn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gqicyuxlo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmpnygbld.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gwuroyyea.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ghlxqyait.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpblkmd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gwjhfbqgm.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gtzqohoxs.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gmoqalcsq.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gdgldnzdk.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gavmandzm.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdaadgjcm.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzxwonslq.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gropezepi.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpynrztdk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gfawqzbor.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gvuohqjqu.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/glfkpgoho.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gcvenhegw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/geogbbtby.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gaemvithu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gvavglpef.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gwyaqbfol.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/geyvitkag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gjwvvxrdj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/goqzbtzjs.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gmmxkzlxr.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gttzbfemk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/grtqmbvdm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcqxhmivi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/grrfbsltr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gkjkoiicv.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gjmxsxbjd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gbinkslhs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gdervhyav.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gkydruwyq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/greaeppqa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/girsxzlqu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gurmifzyy.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/ghmzzydya.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gwgeazdry.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gnlnowwmo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gsxdhgbkr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gtgtbzktr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/grsjrqggn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glgerqkin.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gnzpurjkw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gndrawfyr.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/ggmddabln.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/glfodgydz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gnfjxhiyc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gwvnsgugp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gemdhiqwt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gwuoaydis.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gmnpbmppr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gxeiszpzu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gzomuwqdx.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gzmhvghxi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gvnbcywxt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtnntdkix.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gzaanbrnj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gevihsixx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guucjwltr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gpdatucmt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/goqipmnlj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjolrihhc.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gfrsrvxce.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gfhswwxlr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gbubhixdi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvrhmitdk.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gzjbhissc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/glorxolts.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gnvtlwrtb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gwipwxtbj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gpopssmzi.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gqrysowej.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gihsoqfwm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnftsoxbe.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gzgpxiqcp.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gmdvpervu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/geyhtxcjs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gdvxiresl.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gbopfovav.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/ghdmxbdek.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gmfsetwpr.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gmphchsnw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gxfpywuxw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/guvvgchlg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/ghdfliuvq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gbknsoqii.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gmbwvseau.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gukfdnfjp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gxmuywshp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gwtcsyjpc.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gglpfjyuf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gbgmmvjip.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/ghirchndm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gumtigwjk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/goymzkywz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gltwkvvvz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gugwuicrg.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gqphmkdfl.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gzzjrpxsh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gzghwjqor.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxivpibpg.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsmalfrec.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gvspwmmyi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/ghpzsynry.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gykpfbjqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gzfsxoctb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdoxhscla.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gdpiouvpq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gdujwizgr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gawkluzxs.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gnjrskiht.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gfxzzgjxl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gmkaxcckz.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gpyxjwckt.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gzrccgygh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/grosighdr.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gwwvlvqds.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gcgasxvtz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gpojqwkye.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/ghcoosnwv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gnjmzvxun.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gxtulsisq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxjnlmf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gbgfgongy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/grithjtbe.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gftgkpkuo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/guyxnmcqf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gkikjrvpa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gtxksebob.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gzszqltlc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gvxewbwfi.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/guzvuzfxl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gpxwomdlt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdyrxbinl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gioybehwy.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gssluqrel.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfnkyjqwz.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gllclipyc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpuafdwj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gihfkwkpg.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gxutrnedw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gwxgivnyj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gmmqhiups.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gxjjbappv.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/glggykcdf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gwftobywc.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/ggwkepmgx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gpesmiwvd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gltfttjbv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gfvzkvvox.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlsjyumf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gfppivijq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gnrxpqkyv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gunfrgqvn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gweckkjym.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/glsmckpma.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gyaewoqxu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gvgeuokvd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gjynxyrio.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gwntlmlwq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gagcgsxlt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gxvvunwcs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gpexzxgll.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gyvlmkvbd.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/ggwzqzwkh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/ghesphtmj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gphuhekjo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gwlgxptil.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gkglxrciw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/geppokooj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gbnopenyc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gpmwsnxzk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/grxewdatv.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gyxduhmmx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gmltazrzh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gcfwzmtjl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gunzzhmnd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gpcmoynvj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gzocccukh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/grbphdwqz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gnofxxqaj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gukwqpczc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/glcqhwftf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gnclsldos.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gkilqtxpm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gcddrkbsa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gedohymoj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gfsqsptjq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gcnakovwa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gslnndhtm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gijscoalk.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gckxwziuq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gzivqbwlk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gdvwkqoze.sHtML


<!-- 参考信息 -->