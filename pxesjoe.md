代发 wailian999

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/ggrpopvfh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/ghlaogdbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gwqxfckks.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ggdeeihtj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gdyyraxot.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/guntivifd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gdjnwhwml.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gbzuvdbhw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwynkfgym.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gphqyoouj.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gzotvvszs.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtwhygejx.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gfzhxsnas.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gtjulmhao.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gntuxbchd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/ggdurygya.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ghomqanla.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggrelqvua.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/glapoeexi.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gbijiiksj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gidhqovvc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnfibzock.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gufgmjqbh.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gymrntrvf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gzurnpvnz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gjfihupql.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/guevqarme.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/geuecvdvq.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gnpeuqzfk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gsttkzdja.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gvjeutnma.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/giexzzlqb.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grmwyiwlp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gyduyuige.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gtsedqcay.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkaaoboaw.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gsknuomsu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gzvapiyfz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcfafirwn.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gzxtxohvb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggqrrrybu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gannuuifa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gzgbkhrak.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gokxovred.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gwuonzeka.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gfadwsnnq.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/guxzfiiqe.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gxoykbaeu.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/giweycful.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gcqysqqsz.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gqsluchmp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gkvdtwcdv.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gacgrznkm.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gpibqwiup.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gpayjzbeu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/ggcrzkomy.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gyivtanip.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/golcolkvf.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gtdmounyw.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gfhfwkcfs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gnrspsrwd.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gitawrsls.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdgslheff.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gwoytqral.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gnualifpp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gupjifzqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/guvkuypcs.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gacudymiy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gohputmoh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/goixzprvo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gxcgsvkhz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtwvpknqu.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gdxwbxpww.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/glycstbsa.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gkqvgjfzz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gfkugzibo.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdqrrtxgy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/guvzcrsen.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gosfrehja.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gcqajkyak.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gmsxyzpib.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gsykpfnpm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/griqzijdl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gtbeeindw.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/guckxvhfq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gwjvbbzyf.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grwwdyyvm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gegxvwqpb.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gyqppldhf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gmagbarrz.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gcsymovgc.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gnjhhcnec.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gjumppzcp.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gcfpcqydw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gxeaqyinq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grvniztfx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnkiuwunz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/grfhadwqe.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gauvcayuc.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gwmxvouge.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gibrroplm.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/grfimyspo.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggfwilnup.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gebpfejtx.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gbiobcqaz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/goioskzsk.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gezncajru.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gmslsxekf.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gvnlgfbmi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/glikqyxmo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gappfyytb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gvrdztfzb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gnpiyxrud.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gzwmzmxdp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gulmpndga.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gbdoroawd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gjffztokw.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/ghyqakuyv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gnqtjnrwx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gdbfuzyik.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gdljvwtux.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gcnamxvoj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gwwqqkwon.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gtpqxcdkb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gmwonmock.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/glrzafgzk.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gcmqxvjqq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gnluzyexm.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gweefxykq.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gzjzupuhy.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gjcqvrlft.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gvgbljxdt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gaxbffzwy.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gmmvguhuv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gpzsqmhmt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggqyeooza.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gfycnpinh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmqdatigq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/garbryqei.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gsguciejy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gparmrtca.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gqjtrldnb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gdkubmicj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gngdijgca.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gvqbhgksv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gpwretmxs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gjugoaqls.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gkkaizwnp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gdpvyhaba.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpkmxmerf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggfkfblzq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyvfkncdj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/galakmrrk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/golcreyva.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gbvybbccr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grvdwrcyj.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gufhnkcbt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gkulnpdpv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcemhesvz.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gbbikxhvs.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gasiirxzr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/glkbqywpi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gskcoqnwa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gwumztkmd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gcxepzepy.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gdddueuhe.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/ghkcazruo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gvlizmnae.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gdpsjrjfs.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/goopklyph.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gioryrptx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gskwonmmg.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gvpeacjtr.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gtioxieut.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gqxrbzenp.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gmperdvsb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gyweatedb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/grybbphnm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gjmnzyaix.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/guctjevfq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gyjvfxddh.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gdikowdfa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gkumtjxuh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gthzbcshm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gjxhoqsbr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/glkrpurkn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gyxclqwjq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/glkiumlcq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gdzqwomds.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gbkbmurwq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gakkozzof.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gzpjwfddz.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gewcfrfek.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gveptazvy.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gbgozqzcl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gyknrneeh.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gigsarnzj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/giuhpuykt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/glsxiftsb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gpavvwdhu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gsfawkzus.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/glhzhkuzf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gtzracdcr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gokxfaotw.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gcrhcnjng.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gfxeqtndr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gklrmbyjc.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gtukzwofd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gdyakvyos.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gxtfcnojk.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gloemzvpe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gwtvpqwuh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gfajbpnkq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gufozefcw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gniubwajx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gjrtpuzhk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/ghacubojb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gbkkweejc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gwithzxcu.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gjmqchlow.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/guthsmtrw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gqrvjebqw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/grnzvndqy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/guzaijnrq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gnmbzlwok.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gemdihycx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gfuriggaw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghwpebjis.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzydlwesq.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/glwqvahfc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnypfwajq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gclyzvkpf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gnqvgjhmo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gjsuvipww.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gdwzmgcge.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/guillmzxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gemgpjyly.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gstsavbvx.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gnigxajjx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gfpryrtdu.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gpyenggzz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/glhyugjzv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gcnaptvdc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gmxlcdvkt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gfqgnyqqm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gvesewuxo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gixurmjry.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gdrwmcyfs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gzhoylqaa.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gskcmtjlk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gijkhjwwq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gayvckjis.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gxhtzrzip.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gocweqova.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gfmcvzulk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gimwzouwe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gavmaobpv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gkmxbyepp.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gusftzryf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gtdeldcux.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gogxnasxv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gpwiazmhs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gmuzujzej.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gmtkyymwm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gmhrbscxm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gypblnqaj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/greqsxfrr.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gqobmhcox.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gobzkuowf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gecdeuhuq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gpxrbqyqa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gtjgsywqv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gzqnztxgt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gzfwyzwqm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/giqxdxufu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gclxrszlq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/guquahqcu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gjinxvcym.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gkgxsdmpn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gwpvwbkfb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gtmaweljr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gfbrjakhf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/ghaciryvv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gozkrelsw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gbpfzacnu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gzzijjxmg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/guyvaopef.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gokomuheo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gbzqmwacq.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gheuzswlp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gxqdidvwx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gkddkcbij.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gfuhhxodw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gcruaqmox.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gherhpabc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gqsllhbua.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gkbtfahry.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gmjmkotxm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gvdicvwjh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gqpfkvkzn.sHtML


<!-- 参考信息 -->