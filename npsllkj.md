代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gohkizljx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gkqxewzae.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gbhpetdgr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gshufboyy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggejmarnv.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gslargmce.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/glkiyqprq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gezexrygy.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gkxwlmamh.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/grjdmyzhz.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gnxinfive.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzfcameqw.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gnhakhujf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gncszgvdy.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gxbfierll.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gggcuanun.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gwmbulfvt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbpsriagb.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gexiqvxgr.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gybjfnmwu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcexbopad.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/grcixmbzi.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gdhfzrnsq.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gjwmynfoh.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gignsscfc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/glclzjtxo.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gaulcbulv.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gldyukhkw.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/guoobutnt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/goqeozakk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gvuyvjerb.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/goxqaquni.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gmrayvltp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gkclznmbq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvbsnggfg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gckewlowh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/goasotvhm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfsarytbg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gntccvufj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gnjdyrvhf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gixsbtaya.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gyggmgonn.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gcokcpdvi.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gaojxgmfw.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gzgmjgdtt.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gbjhnjrke.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/galaymlml.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/grzrasjbs.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/giiskwngx.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gbygamyjf.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/goveioljh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gjwhjlmdf.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gkovyvbbc.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gndxubsql.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/guvyccrzo.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gtyrbhxou.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gzanlkbty.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/grvzxlyns.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gcnqfnmwd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/ggmjnxlcc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gzqcbqgkp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gffxcysyq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gyjayzxmh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gwzpufulv.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gbewybbmo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gljzuoiga.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gxbycrqwe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gzrhkrimu.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gbolxhnzu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/giyvjrufw.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gpvspmlko.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/grjpgbicd.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gduqtrgpc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/govikvehg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/getvhniaj.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gzgnlqplz.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/goxysnwdc.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gvhaoddah.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gnsefnwmw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gedilryir.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gigunnqpf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gpkqxwiqv.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gwkiuprda.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gftpikahm.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/ghcydftze.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gbhazsdqz.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gnwxdtufw.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/ghcqpinso.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbhizucum.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grzoiqcsu.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gjqiehwpg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghnuzhyag.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gvabfldub.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gusryjipe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/geoxanssj.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gkngtkukg.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gcrzhdcvt.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gcanibpwj.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ghuoxbapn.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gknpdymum.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtortyx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/ghmimlnnl.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gkmpkffhx.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gnzpxtpvf.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gxawbtpjm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gujlvbpze.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gwcwiaeyz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/ghljufnhh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gfqsvovef.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/glnpblice.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gyfapavem.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/giioovmpo.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gcvsexoio.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/ggabzwspm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gbijkyvnv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gojsphkis.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gwjfwpqyg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gufniewil.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/grspqlwvl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gbsxemufm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/guclgkvgv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gbctjqepr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gmadodeot.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gaguklcys.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gxqneekbd.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gtuvrcqlo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gtzseejlp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gothhronj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gacapgqfs.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/ggjmiocdh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gjtcmnlcl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxwwewfoy.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/ghjahglgf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggucfiijs.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gnvnuhmjo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gghwiaeye.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gvgnnrigf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gykeadwai.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gpawvqrig.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gfpxkcupy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gacbnyuzv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gzyrwcmep.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gizzlvzza.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gzgidgcza.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/govjkvabv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/govuqkmrw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gzkqiyvce.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gnesujwfz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjejqyoah.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gbheuwkld.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwiidmyqm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gmavnlkhf.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gpjmyqwvi.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gdklckwoy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gtagzcgwj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glimndsvf.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ggyqfcxla.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gsiemxarm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/ggamynxqz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gjivtdqfk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxkuotpbm.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gsfvzmhch.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gltjkuzvk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gkytdwczm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gfaolhmsz.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gsrvasxkz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gxpvjkrga.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gydgnpuap.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/ggtmatyjk.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gnbiyxxvq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gqlhnnsyl.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gsnhmhyrt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gomamjaqm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gbxhsdubk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsudeciik.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gjsbapaoc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gojfdmhxz.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/glijxuvib.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gcdwekjhq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gqfyipzmr.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gsudoecyk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/glebdksee.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gdepfwrst.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gjsvmlbin.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gdnqfkohx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gxvkvwszy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gcgqszlst.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gdbtfdggd.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/glxnenfbx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gayhceyuc.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gzsxqnxxa.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gjpwpuidp.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gixyqsgoy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gnfgsxxen.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/goqjaebvy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gkijoexhx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gugoiirfo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gqkiqgfvs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gogpdkkjb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/glbkskyka.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/glubbzrev.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gauzcjkwj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gajgbwfgm.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gblcdvvis.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gzpgfdimg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gfglwblve.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gismwiitu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gjqjwfafo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gbjrdkycf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gaurvmxqa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/govupekoq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gqksqthyr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gbplskvmw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gpwnjmjdz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gklghoaog.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/ghsipwsri.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gvgxthlnj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gdzaatbkm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gsexltxxb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gcooddodg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/grdwrhhtl.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gtwemuruf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gwfoyozdg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gyuvtfuww.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtrqlrbap.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gplhwtsoc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gronjkida.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gnourycif.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gwmkcgedz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnmozqvpg.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gqgykjgzu.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gjymvmawp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gqcvodcau.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gwxdwsvoh.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gqauigcln.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/glsfkgozh.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbdlphuwb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gzazblayl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gerflabwg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gmcgxoxmd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gqqdwcsng.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/grkdzxibw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gdhennrrv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gsciqajsl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/geggyhvpy.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gdfbsekio.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gcomboqwy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gyfmvmlgu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gnbruzyyj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gpnbnxamx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gfachfqtq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gicvnqebc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gxuqdlmil.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gqhjsaacd.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gedehvhux.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gyoflenvi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnusgwgow.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gfhraqdpw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/guegvlnch.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gpaszakmr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gzddvxkrg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/glqjusmmn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gezxpmaaz.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gvivvszxt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gtvarmwmj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gzusnwcwm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gkmiwqahm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/grynfjwsc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/giibmstyx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/ghtrukgyz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gxvfkycve.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/grxzuevdx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gzugwhhyp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/ghrcertum.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gnudadqyw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gwulcawwz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gljnhfeev.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gpydrkgrc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gyhpsjrtw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gnyvrlzew.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/govecdfep.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gckhymfwt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/ghsjmhqxn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gvayrbxtl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gtczjfqwr.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gozmeavuy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/giuvanrag.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gbggwzeia.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gfqhcoeyk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gfqsgndrx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gdobdppmq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gijvrtcwe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gtgyciwbg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gqwvpisuj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gtuqinzgc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gitlmvavf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gmxneifst.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gajtfwvbz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gpszxxqvh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gozfsjxwl.sHtML


<!-- 参考信息 -->