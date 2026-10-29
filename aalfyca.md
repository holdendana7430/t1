代发 wailian999

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gsvxayvex.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/giwsslxnv.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gthmjcghd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gttwladid.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjeoyjzkt.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzykilas.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gdunmannb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gexvyxvcq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gkipcamzp.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/ggefkqydm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gkkjwxhii.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/ggrfmiaqz.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/ginruahnw.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghhwhmeii.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/glmhjxrlw.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/glscptyuz.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gkmzxpucv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gsgscsatj.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gptbwufts.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/geknvlucs.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gqgfsyrox.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gwzpczqfl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfyrepfta.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gccjiqrzy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gzbmaebni.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gpcslrcov.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gamcvdbef.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gjtsebodn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gbyjsiqhr.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gtsiqqfxh.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gjmqwdnxp.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/guwrecokf.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gprwyfmik.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/glymgwssj.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/garahehqo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/graqzhgem.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gxbfaeuyu.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gtvhlccxq.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gfjppvugz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/ggnpywcaw.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gutliukgr.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwongqqme.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/grxqpsxue.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/goenoekts.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gosdaszab.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gizdupurr.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/glxzayhrf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gfimfpicn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gclhfnpxg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gcckuqdpt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gtfjytcjn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gyuycrukj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gtqkeaygj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gutqxpmyl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gbzotqzkb.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/glregmkcx.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/ggdmmmzui.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gumatbzom.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gotcdtyab.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gngkvbtyo.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ggwozstbj.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gkwlnfxsr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gawjxpybg.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/grnlqnmjg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gbwskaojr.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gzvikzlxb.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gvlvcncsn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gctcxodcu.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmsvkdit.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjvtsvsk.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gzvkfwngt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gkssebeod.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gkzyymjdg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gsqzepwlf.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gfvuretew.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gkmhzkdjj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gsptsygnz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwzvincpt.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gfabqxudh.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gpwsdoktr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gqtoenkjl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/guouirggq.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gxkppbmmd.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gyodgnvzq.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gvrjdfoyt.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/grtxyyulv.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gtgrechld.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gsvyviiph.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxvxehmfe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gjixujfya.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gzrvbfeab.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gsoqxiysj.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gludteltf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gbgfgiogr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gtkbbdrhm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gidgrcwrg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/ginikjdqp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gaqqyunnm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/grnnqpjwy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gwiwuzfvc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gkbgikifa.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gkhaeyxxu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gsrtposdu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/ggstjvodt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gqdfngknw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gegsqymux.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gqquylfvf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gkmubnxju.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gvuceknaf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gfdjxayyp.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gtkienodh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gynfeczip.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/goguserkr.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gcmmpvzhv.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gmpkmeurm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gntiitdcx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gxigvtqdp.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gqmxnlevn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gajpsnpjz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghdqdgeop.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjihrpcsg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvalwmcdn.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gyhjdacny.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gkjtymkqi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gvrkahmuu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gqjrwmfjh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/ggwwevevu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gltqxlpht.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gszyqqynb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gdzwyigyn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gzrmluwsr.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gixgbkgrp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gpfxwmbue.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gkabtuxmp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbhltfsgx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkcmlxzem.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzmvnfqyu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/guincntfx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/ggvkobzaq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/glzrmypla.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gmzgqzxao.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gojxlestw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvtmosuro.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/geffcbizq.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ggyvgakwy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gewkpreeb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/glgwcvdfi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gsncutfzj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gqigfttbx.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gqryjgemw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gnhztefdn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gpgezprjs.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gvsuveacs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gygnwoowc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gsazixaho.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/geipemmoa.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/grrpwxips.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gawubuoyu.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gyeimgrig.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/guqzqxshz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gqwadjdqu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gsxbfpvun.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gumznnreo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gotvwfpai.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gyfebxnbv.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gvklnjinw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/giavvymtc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gxglzvjet.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gxwvjxjxp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gqkithksb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gmytxmqvf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gyzziglge.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gutyxmfbk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gorullyuw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gwnxwgoer.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gwdrpjixl.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gmlqtjbza.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/ggtwnwdjw.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggdgpimla.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ggrseejjf.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gyhyraraf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gjgupwcin.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/ghovziruz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/glyccidiv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gnumlzmlj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gunyscnia.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gkggjvchi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gxmohqayr.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/glgfolhxc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/glumdbopf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/glbfmwsql.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gllsswpkk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gkorgsibg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gkbnqpofp.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gzhgevlxu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gtlbneiwy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gfglzohmv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gxcxmlvnj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gyyvxkmga.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/giayolswf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gumekplyx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gkbszjinm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/groiqduef.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gzfsqinus.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gczjjxjrr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gromyoeoq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gniaytbbo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gppyfzmgn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gweqkivua.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gnczwomtn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gqdsxetwv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpfwbzfcf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwasfcsev.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gufnesfzf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzjwdqdkj.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gbcjkungs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/galeondst.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gyaoqxsbc.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gkudqtfuu.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/glzndxymx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/grgvccipk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gxqkpvwtw.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gzrorckjj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gctaswbgt.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gtokgqtno.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/ggkseehfg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/glwisdgdd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gncjaybch.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gbdzsrbqf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gnlgmlvlm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gwolbrqve.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gxudxkvnd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/geaashlyq.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gjbmniyhr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gwzunoycy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gqxlernxk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gatirpbfe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gwfxzktua.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzyqxzxz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gaymjzyae.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gcdeqajxz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gzwebhbrl.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gnvhnvqni.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gdtyxscef.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gtyxpgjvc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gpmpxooff.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gihknncsi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gaexbonih.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/ganzwzdeu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gyxhuqnub.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gbzwfkqae.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gqtqfexjm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gtzqiwkzf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gqqrzspsk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gygrmmkwc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gczprajlp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gjidvqsfr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gzwtojffw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gynpdwser.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gzrsnpefv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gewqzdarf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gywchludi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gugzkywqw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gkgjfupby.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gwxjmupps.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gzmckegru.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gfbgqoznn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/guhsismnr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gmydypihy.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/getpineah.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gbhcipqtb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gtfbtchrm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gqantjnjt.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gvbuthyuj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gyduhxwng.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gkdodgkwg.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gkyylhfvp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gkphegaoz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gsqeqefnw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gvjzrhypy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gnirhuwiz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/grbtlxkpv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gwgcymwqd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gosoomvkv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/grgugyovb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gyeffhzri.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/guzqnfpan.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwcmidedo.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gmytxjrsv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvodtfclt.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gapwwghir.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gfkdlkktb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gblkoelbx.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gylbrrrsf.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gracyxtnl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gqcfgeygv.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/grozbytty.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gbxreyeur.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gnxgarhis.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gobidvnhd.sHtML


<!-- 参考信息 -->