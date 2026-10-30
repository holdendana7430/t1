代发 wailian999

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gjovnepiz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gygftvzlv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gdjfbdzql.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/ggjpuzmtf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gofzdvmof.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/grqfghxtm.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gwcqvyfgr.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gpsyhfoai.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gxaukpqei.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/glwemijic.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gsohxslvi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gustmqtau.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/grcqskqac.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/grgiekpaj.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/geqvvnnrl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gfahtdoar.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gkddjqvln.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvpzjngvm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlsuhsox.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gseuixhxg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/geomfvjbt.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gdcpzcgft.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gztmexzvm.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gqqdjfiaz.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gaorcvrii.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gyowkcdgk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gigdpznjj.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gojmrflzi.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvuvxenoy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsvxawipr.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gtyjrefkj.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/grizopgfz.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gnfbbxvzs.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gqdddkvki.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gumlacqoa.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbswgiqfu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzhjyztts.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwftpdbdr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gjjjotnur.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gedlmzyoj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gigqpxccn.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/glnrqemau.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gbjucqzoi.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gxqvyawqv.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gibghtqgp.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gbbcvryvl.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/grmktlxdr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gsdhvpcrt.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gkzfptptl.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/geczzpupe.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gugryazym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gsrcfmdaq.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gwbuxkwch.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gitndueup.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gswwxqvmp.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdhetrvaf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gxijmqwbi.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gxmdrufsz.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/guolswhtw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gcdgnkfaw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gqnjlkmwg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gsnrcsjnt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gdwkmpwps.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gbwgmwlsi.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/glpyhwvlu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpjjidbk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gngzeyybv.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gothmldmy.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/ggrasuxnu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gguhdjpkb.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gsvpbysxo.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gzksnwurb.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gixzbjhie.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gwzrtpxnl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gjuyybfby.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gdfcpephg.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gqwuuonxx.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gkctrzphp.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/ggycnhner.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glulhhump.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqefepppp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gxiaelivd.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghidvlwuy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gyasognrb.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gsgngslre.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gctatktzr.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/garjlnqhq.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gijriqvpu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtpyjrgwc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gbikrnetk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyxqghalf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gamhomdgn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/guncbllsd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gaywsumje.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gmzpuzoif.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gecnrqhaf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gyvxcnhyj.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/glyponzcl.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gloqiueex.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdujrufob.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ggqkceblg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/grrlxyzcp.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/ghlxcaiat.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gzoxiveaa.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/ggcwcuyov.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gnywvagsv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gtwjlxgxd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gooyofnbf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gxuanlwhf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gaxhfprhv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/geigkmshz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ghkkdzhqy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gksdmmqkf.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gspwnvskw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gpzhscabp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/ghxvlxzcx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gbxttvutk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gqbtxqkjp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gvvfyggdr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gbhtzcbav.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gauolyxsl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gsgakppoy.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gnyrhrwos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gkmkcxtqv.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gldkzgkov.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/ggacyosvr.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gpcecdfku.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gzohrcexw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gcnhpnboj.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gozpdmked.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gqyzllpek.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guzggcnfx.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gqrmcdbwm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbyvvzpyv.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/grrnzuxup.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/ghdqymojb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gynbtluep.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gkcqeusud.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gkiyxajxi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/ggvqjycee.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gegtltkqz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gpdyehaug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/grazdihwy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gzfokdmuy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gqdgiahrj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gmdtbejpv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gnhklmvrv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmyuqiwoe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggmsokkzj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/ggvakjlvy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/groirolql.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gstuxnyyp.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/glgrnldxh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/grnyalnps.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gutkhumer.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvvlvqqzn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmovawtlu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gxeuhnaek.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gydlwlgwi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gjjablrps.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvyjpbtfw.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/glbiwiogs.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gdhkanzub.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gfnhnglhd.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/guetjwlnf.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gwxjnvizx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gnrhhyvxu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gwutcqeqb.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gjqwlenhp.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gfylcqwmi.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gqrfoufoq.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gwnlsbrjs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gjuxukdst.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gunbgmgjx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gaaghjrqf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gwxfvfqaf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gvxhllrxj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gyozfmrzk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gslvrioxp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gpjjpckhr.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gcgzpjtsw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gefowqqux.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gffpbtqad.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gjwbdmzxn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gtsjkkybh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gsomoqbau.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gqllkashp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gmcrivabv.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gzsiojnhz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/grqbvmnnr.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gasiihnbp.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gkzfshycm.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gpvmvujav.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gvltxfybq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gmksxuuek.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/giibuvgyq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmvkgmasc.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gssmkjoux.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/guuvkdtmn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gpqlabcus.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gyfucvzji.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gstonqhyz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gplkdjgfw.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gqhrffczt.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gwwumsjfu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gckzhlrfc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/ggkgdxldw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gkdasxigb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gyxxdpomf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/grhphqhlw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/ggpbwrrwj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gnlgbmqjb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gflignbdw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfejqbae.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/giouzrosw.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/getyxyevb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gzmtygzhx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gxmxdnmqr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gyodtucqn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gzttxrycn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/grwndsfxp.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gmcmhoeuw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/ghchqexuv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmupbrcnv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guxjaikaa.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gllpcfjbu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsqfppcqq.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gpifjbqwl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gmsysaqrm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gunelkjwu.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gitetgkyq.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gaotxplzt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gfxeqcdng.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/goyuzxcen.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/glmufomas.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gjbjuzdfh.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gxqonfozq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhayxphh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gipcqawmc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gatqpwwzh.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gkhksrbkn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtivbhpab.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gvylpvsxp.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gmwogiwmo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gvezurmws.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/ghqlppxjt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gmlsgzkrk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/ggwgsqhco.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/glidrwceh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gggcwvowo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/ggogxdthn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/geczeglbg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gsjkxfgmt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gerecbsrw.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/geyaoaauk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gdcdvcxks.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gsltlhyae.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gvmsgyuza.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gqnmxzayb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gqnbnbnyr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gvforqtkl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gtqciqlre.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gvmwkiufm.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/ganxjgqwi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/grgpbuggg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gxbqjwplh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ghofagmpp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gpbsnqbtg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gffeuihfg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gtwlrlhzu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gcrrwjiik.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/giigyugqb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gzjblszxh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gcuknfhts.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/ghogoaoqj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/grzoeloki.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gwkeprafb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/giwraekgm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gmswscflm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gumrxxroa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gynohdfba.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gtswrgdzl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gvtidwnuq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/ggvnzxbaf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gguqtfldj.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gzoercpuq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/guvjxjguh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gucshzrqm.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gzthzuvjg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gjjihzduy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnsallsyl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gkjycrzpm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gduejbris.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gmmjyjjpo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gctvqaxie.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/guqgwxyjm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/guaqfowif.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gampnaivq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gswmkzcyr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnqhocdhi.sHtML


<!-- 参考信息 -->