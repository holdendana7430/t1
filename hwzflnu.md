代发 wailian999

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfwnkhuyg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcauswrq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspqnuivh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gctlkitoj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghvitmekr.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrxzslvy.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaapsmruh.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geynnhxdh.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooqaaopr.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaetruvxr.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/gobexrizd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhodshqz.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzoyofpq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gbpwfnfsd.sHtML

[G04] 定义方法
来源：http://3g.fanxiaobao.xyz/Article/details/gzbbrexdw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gvumuwulp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzprhevc.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaedpgoa.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmelbsbms.sHtML

Java: String greet() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmhntjli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaucsbuf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqccxzese.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkoiemgu.sHtML

[G05] 继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyavexox.sHtML

Py:   class Admin(User): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gksxolzdd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbknovqvw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxhnqbnr.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzcqmvifd.sHtML

Java: class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gylkoxoeb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrnfxkvp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnzaloml.sHtML

C#:   class Admin : User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkibxgkxc.sHtML

[G06] 重写方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadtsszfw.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpakrvuhu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviedkkla.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gohdocxuq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvfzwrhm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvubrdmz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqrrkhip.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsofjtzr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhzicmxc.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzmtmgif.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/gkcpbpogj.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gtfleogfw.sHtML

JS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gkatyuzsb.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqoafujy.sHtML

Java: super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqvcwrvc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fanxiaobao.xyz/Article/details/ghuzacbda.sHtML

Ruby: super
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxtdtjbu.sHtML

C#:   base.Greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuqmleqc.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/gkortzcym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fanxiaobao.xyz/Article/details/gahkggcar.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gexvrkxfi.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmllxlxw.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfoxqehz.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggechfumq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fanxiaobao.xyz/Article/details/gwbsubxkv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvwtspbh.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtjslbqi.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwcamnlb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuddqsok.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhomrpav.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdorzdbp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthrfnzaf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrryztau.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/guxvsqgeo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/goexshdbs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjcwibpa.sHtML

[G10] 访问控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gwerarbig.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkewqfyvl.sHtML

PHP:  public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/ggivqfljm.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gbneaqebx.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/ghuyfmwja.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gxmcbbrht.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgebisrz.sHtML

Ruby: public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gghrebsqi.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdimnipt.sHtML

[G11] getter / setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmjahwqx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fanxiaobao.xyz/Article/details/ghahtibgg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gldsmntfq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnijhguii.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpxcgsbad.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljsxgkcl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktmfxvva.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpnmoqtr.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guqetzcze.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsydpdum.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhelnxqv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gseijsfcc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggiuafrfr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrkrgzbf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbdktvqh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgexuxtp.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gxwoackgb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwxfotiw.sHtML

[G13] 判断对象类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfpfrujix.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmckehqgs.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/grzrljtth.sHtML

JS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gzpgrlgxw.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gxnsseqss.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdzyjqne.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gngdklogl.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbuyyreb.sHtML

C#:   u is User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcnopobc.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/gsvfuxorp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fanxiaobao.xyz/Article/details/gqnaunzcb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gebbgtjfl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxlynoki.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdbqlygn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuyktfdg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxmeocqw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fanxiaobao.xyz/Article/details/gwocpbtcc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gjifuzdse.sHtML

[G15] 枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gmcwcjzsn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcszubkyw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmahjxic.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvydypxu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejphzloq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fanxiaobao.xyz/Article/details/guluqbbzh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhnjmzku.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gdejgfbld.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhuoerc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gullkgsrz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/gbrtqaxsd.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvvrwscw.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/giyotpigy.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/grvmrnrrc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gmmyebfpp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gapjaxabr.sHtML

Ruby: obj.instance_variables
来源：http://wap.fanxiaobao.xyz/Article/details/gtbzbwauo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawrcgdjp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbgggdhh.sHtML

H. 异常与错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/guocgazqa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcxquonhn.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/gvbmobkef.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gfyjgokal.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gegujxzax.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiacryvb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/grllpgtqr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/govrvpafd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fanxiaobao.xyz/Article/details/gfutdlwhf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fanxiaobao.xyz/Article/details/goxyqooof.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoxzhsik.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fanxiaobao.xyz/Article/details/gvcgruchu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajatuxcj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/godqtvqvz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/glazfkkke.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaemhqubc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuqhmduc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fanxiaobao.xyz/Article/details/gfrakcsvq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoirwmdi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzuanahx.sHtML

[H03] 主动抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gfabmhfsi.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/gissaqdta.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gkfmvpcnr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/geuovepxb.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfsiibhh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/grfymgfbq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaejddzcm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjjarite.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnczodqw.sHtML

[H04] 自定义异常类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdysmbmco.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fanxiaobao.xyz/Article/details/glkwhbsvb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdrfckhh.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtndjzwhb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/glqvejtzb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjzdtgkmh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbiqgrxg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/gplavprlj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gymajxoev.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdrpdncz.sHtML

Py:   except ValueError as e:
来源：http://blog.fanxiaobao.xyz/Article/details/grknjquhc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gabrslksi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkzemtps.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxepuolr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gluchyvuv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fanxiaobao.xyz/Article/details/gfropzomx.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fanxiaobao.xyz/Article/details/gldtizqaf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxpkbhuv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliwqmdqn.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gmeerxfmc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gwwbrphtw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxzacbcd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/glhczvnvf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/gpuueijry.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/giyblsqtj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fanxiaobao.xyz/Article/details/gjurlfuha.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/godvnwyxs.sHtML

[H07] 断言
来源：http://baike.fanxiaobao.xyz/Article/details/gplcszojs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmnbcbaw.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/grggvfrcx.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzqbehik.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyexerrq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fanxiaobao.xyz/Article/details/gkxwmtpqp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsqmadfd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gucixynmk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdrdkbzb.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gdltavkyu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfsggrbw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fanxiaobao.xyz/Article/details/gzaeegtnc.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gqohzhgnd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrbtljjq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemqazzqi.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gqphcfmqj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkzebikn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeyuccbj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdawxmip.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/grrcklsrh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmartadn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbdqvlia.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwzcswuny.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzepxkdj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gmxruepsc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fanxiaobao.xyz/Article/details/gfqmzlqiv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnalhsptb.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gtjbnagyr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fanxiaobao.xyz/Article/details/ganajotob.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnswmemri.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfssxvjbz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gmlgwsgtz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/gfkmfvfzh.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/gavngxwjl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guetujvle.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gloesfitr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guxoibjpl.sHtML

I. 正则表达式
来源：http://blog.fanxiaobao.xyz/Article/details/glqafosjv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwjsjdjw.sHtML

[I01] 判断是否匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsihqtndx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtfdxaku.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmgixzlf.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gmqslkurh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnansacy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjlgqzgi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzqeqamfp.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gxrakpwzw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaftnbla.sHtML

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyrjubwq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcidsitbv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggovzmzmt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhaqkomx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geutvonve.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gjihgeotf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxsrkajh.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwawruuwj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gqgmltdpt.sHtML

[I03] 提取捕获分组
来源：http://blog.fanxiaobao.xyz/Article/details/gfvqyrndt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfihglsco.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlhdyqkg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gegfsxeqj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gqjjfermn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrimnuki.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/gjsazgczt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gzchkejif.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzmizhgn.sHtML

[I04] 正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glzqmmhnj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gicujaush.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/guoicdezy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcvymeku.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmljhbgod.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsswqulou.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/geilythtb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/govppbnhu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbivhncm.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcmgxosk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdrhuebbd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gnpjimslw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxocvatp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gjaqhyrzq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcocrrijz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjmentmpw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gbmmcbiqa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/gjjjpfxwt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fanxiaobao.xyz/Article/details/gctwkvvkk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/grpadvaku.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fanxiaobao.xyz/Article/details/gcvqcspik.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozlukikx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeuzcfxd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrhnceyw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfyyrfpo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpqedqhh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gknzpvkgk.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gteolavar.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fanxiaobao.xyz/Article/details/gaebvqhdo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylfgolxp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gnkgpxuug.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/gtzwfiqwa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjiigpkv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhhkiyub.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunhpecb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fanxiaobao.xyz/Article/details/gdthnhpez.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzilqpgq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fanxiaobao.xyz/Article/details/gttlqcqlu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafatwbra.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeyvldja.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gslzrfjrl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggijvpwza.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgpxbfzm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgeknqss.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejvotgex.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsglaescc.sHtML


<!-- 参考信息 -->