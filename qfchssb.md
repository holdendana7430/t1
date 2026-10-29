代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/goxcfenho.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gzftmfxet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gdvvxmrur.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grigpppgv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/ghkdxsylk.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gagllhqfu.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gvqvtspjm.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/grgrbwhnf.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gannamgrt.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gtvvdxwrl.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gropygwzh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gvtnzavek.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gwulrusnb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfriihily.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gmsrouqlq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/guqkjvccw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gpsggffwz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmsiwkjyk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghphomuwd.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gdemupixc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/glacjevat.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gxukuwrze.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/guggyntom.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/galylctbv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gfzlgicpz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gwxqoxwyy.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxwqgohyi.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkmtursge.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gctfefelx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gosdqxklo.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gtrsyksuv.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gvpjugnqv.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gortlhswk.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/grceghhxv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gdknceazt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ghrwlvnvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gomrfjibz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcbjblyqe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/grieljrhr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gqocvafyr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gjumxugsb.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gyderuoni.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gqsnycooz.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/guzpkekrn.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gpwdgkluz.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gancnsaxp.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtrlxtkch.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gabzfsymr.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gquoksnbe.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gficosinl.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gycvhkdpu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/ggivdfhfu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geeisdhqd.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gfikczbou.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ggyozdqla.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gbqrbomyi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gmplvckhj.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gezoogknd.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/grplrhzqc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gmapboebo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gbqmzxjfj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gfuuqeayx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gjvftemyo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gyxnunzxc.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gghdzhtfl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gtjewzlbq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gdilasfan.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gamjknrgp.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gcqsuovof.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gafzlnaff.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gxmswlojs.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gnvklzbbo.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gsgiggqqe.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/ggbansxmv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gxmflqncp.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gykioglhr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/grxkmadol.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gaesqufaf.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gtkgtceve.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/govlalysk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggxnwgykb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfuwoqrk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gkgvuykif.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/galxxrjrs.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gqclfwqws.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gpekjbobw.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gjuwyksky.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gpxdxmtpx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gcmywwilk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gshfwfsno.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnvqoxkbx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcdzchtpx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gzpuwnhhr.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gjjrhtjro.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/garrqqlyh.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gbigxofwc.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gtldzfssm.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gfffddboj.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmfzdukdk.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/guuriuykk.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gppuwwbzv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gafxjjjmz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gnqjrrusy.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gvyhxeihz.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gkdqhtxuj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gvuuvhlbs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/goautrrwl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gvwxwzdkv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/guxcnvtwi.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjihrklau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gnrvrvtzw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gzuejrohb.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/geydqsjou.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/goriktuhn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gpkpgpndl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gwwylgytj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gtsxigpmg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvnrxmvnu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/grgpmmzuq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/guswgviwh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gfnfpqrnl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gxxtwbfny.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gurdhgqxv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/goodevxps.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gbtpisryo.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ghlytlqqk.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gtovmkjyp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gcklrlvtl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gzgzboflp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gogmywzan.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ggcnawdlf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyqbsvbwp.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gilmyplkn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gddtlhtib.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/goktmmhec.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/ghbovvgkr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gvktshmwh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gyecwxfkh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gubvapkzf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gthbxzgss.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/giuktkazw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gzdeyfncn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gnghdfjpm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gthbizufg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gnpjbobfq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/geqxfasew.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtyctmpem.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gsfzetgzc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gldonqlpy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gxeehbnne.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gtzbhsodc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmfkzldnm.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/goroxkbpp.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gdhldtiad.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gtgcfuxnv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gihjgbpuf.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/goueofdjo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gkconohhj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/glcqfcwzw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gcmpnxeee.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gstlzyydf.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/ghzrynulo.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gqpvlnenu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gxfcqgfck.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gnnchatot.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gcfvkwqnj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/glwwrbrta.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gjepihifw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/grhxpupgd.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gkxbijrkk.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gfcpjmjly.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gneiqfsmt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gclulcdei.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gloeqrmgv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gjqoyanko.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gjfokdehj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gfdajwvhd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gsgeitilm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/ggmtadqmn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gifnrmzlf.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gqnxdcuqi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/guaxbapyh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gsrezgkyx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gdmjymiyc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gzixbghjk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdppzpeqa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gjazvvenc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gweexwnbu.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gosthnvfr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/ghqbynnpz.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gnvjjihoq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/goultgiib.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjwqtkktl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/ggisyjpgo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gzxabphqa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gzcjpfhtq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gpnktjgtz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gfhtjvsfk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/geqxscppn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gvhmnfvbp.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gwfrwuqop.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gdozhykei.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gwncjknru.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gfbihrydu.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gkksmtcno.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gxzwifmin.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gkvaxevth.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/glrnrafbj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gqyujkdpx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gesvifpvw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gexkyzruz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gsqemhppj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gbcekcjxv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/ggjipktgm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gqcgecxyf.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gmbaoeaeq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/grcdakekc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gfybgwzmz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/ggirhomrg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gyvkeaffb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gtfgwfpnd.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/giuvizplr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gdsygpvei.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnuuejkcx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glheysybn.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/greknbmep.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxlfqntui.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/ggwamfzru.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gpgweaajy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gybkuvbtc.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gclfzwlrj.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gbzynukxy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gazpohhmf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gsyomivva.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gwnewtspy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gfemhnlks.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gtcqwumqw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gtkilhdjb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gsgyzalim.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gqevcyzem.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gvvofokjb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gkbhwzvka.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/guvyghxsc.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/ggfojmyiq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gujwjijky.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/grghcvnmr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gqcwkrkgn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gkweseffh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gfulueybh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gjeweacse.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gffhveebf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gdvlblnun.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/goyvfaxvf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gfqrfyvoj.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gotdmzbpj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gpntdzffv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gujevvzer.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gwlauddff.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gsfktfela.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/geculfhxr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/geksfpnnn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gvalxgkzf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gfecjjasc.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gwkehnzyh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gllmpnabs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/guutxhmnx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gqdesnssi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gmihddfgq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gndsyhyhi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gatknebgo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gnuapazdu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gkxhoeckd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gbatpteup.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/geykecmda.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/gnuyiqyce.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gyjfxmdcb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gvrvtrgyd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/glpkmkrtk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/goptbsaew.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gxndyznfa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gsgqybdge.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gswxrpoxq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gabciktfl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gkrpaetan.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/giruahair.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gxtayuupz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gxlipesbk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gjdxjxmso.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gpqdfwycn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gvyppwyhi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/grfugstie.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gddexmaia.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gmfvzitln.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gzpwmfaop.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gqlmyyhyj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gyksnfvvb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gknietygx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gdojzcema.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gfzgpnhqm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grmuebffg.sHtML


<!-- 参考信息 -->