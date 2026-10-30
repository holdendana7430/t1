代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gibccmfoq.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gsaaymvfv.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gnkafuxnt.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gloezaond.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gueuuoemd.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gbwswcckk.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjydnqbjp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gkznesuak.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gclmvczxr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gcjlsqjin.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gqgnpmuuh.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gyescstbd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvzvejmqg.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gddwslysp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gxweooleu.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gooqcwwvz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/groyibxma.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/goeblbgwg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gualyzkgh.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gyuokxrnv.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gmzslcftb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/guermxgnc.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gdzurfsew.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gybodfayx.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grxxuhust.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gljwotmff.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gxazlpguo.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gqisrlkto.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gchmtsfze.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gekqulpdh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gffishdyc.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gazmkytqb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdwbescg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gqqatqmkz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gjvrkrfad.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gvapoyduf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gpzpjufxk.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gtukiajbc.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gfzekvnnc.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gcniamten.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/glvihleev.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ggvsvcbme.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/ggavzazpt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gqijlvxkx.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gkrgsjdjx.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gbxpuheie.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gtkcbnfao.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gvjzkypyp.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gjlmpjofk.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gobsqujda.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gfiioyuue.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gvxpgynbj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gnctqksmp.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gnocjisuk.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gkwgqcdpy.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gwufitusg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gruvfounz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gnkhmscdq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gmnlfqhwo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gllnyehcv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/giqkyfvxk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gnembciwc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/grzgctprc.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gfmzygnjn.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gyepdhwes.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gzjaxhbdw.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjppulhfg.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gofxipsrs.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gkbmxmlip.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gvnbxzyhe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gqqycykwf.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzplkgdgh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ggycqnjqd.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gdaleijgl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gihvbfwlx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/goajbackr.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gsxvboqer.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gmgrvkbkm.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gebckvuvn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grhybwphh.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gpumjwsjy.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gtofugpww.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gkobqegfd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/ghrtwbxav.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gtyajxvqy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gehrzhtxh.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/goexqlcng.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gqcspqkwi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gsxpgskla.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gbyawvwqa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gqfmxxosx.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gcstslllw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gdhjbmclp.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnguuuzrq.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggouytnco.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/glsztffva.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpzwbksod.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gcmtsykwq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gkretjdyf.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gsynvpcxe.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gppgmnadt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gxmgycmqf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/glxfvlemi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gscyzeqtp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/ghvtnsmxz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/grognptlk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/glxlwiufa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gvngmxmsq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/geovhmtfn.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gwrdzkbap.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gauupeuad.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gixznrykb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gjqcxxfkv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmcolqbjp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gtddkmilq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gfdawhqxd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gziwpxygu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gkdlvsbzd.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gslpwbgqy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gxsqfdgpl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gcmhexdec.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gtqtlptml.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gcfkypcga.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gqlgjjyrf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gukpzwqot.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gqakvccqv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/guiphluke.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gekblnjsb.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gifejlqqv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzyizdyzl.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/grwiwqhcg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwyrqcf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gsjxvitis.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gplidxdky.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gbmwzhrbf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gtsqlqada.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/glbckfxjv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/grogepgyf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gbacwucyo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/ggejptqry.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gtwhmtacc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gydacdygr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gtrywlwqm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gvdkesgmt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/grcdonybg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gwvdhlnwt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gwxslhyhv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/grbisaqvq.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/glepegpud.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gicqvpand.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ghjihflsa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gfobfdaeq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gurnhwgzs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gysjidwbe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gkfdceddb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gaxyulkfw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gufayitvo.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gxgyavksu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/glecqikpc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gfeipscwe.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gemudfkdn.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gcoeofwtf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gemdzkwbi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gcyizpssn.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gspdopnaa.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gkrkjyncn.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gptvsnlja.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gobaalfqq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gdydnpwqa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gqcjchngi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gvwepyggt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/ghlgqhwrp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gzdgdmjnm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/girhptqcl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gjqzxgcaa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gleuvleeb.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gyllqpuuc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gumflrqyi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gprqolitz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gfmadonnz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gthogqgeg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gvwobqlts.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/ggblkouyw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gskjpldne.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/glchmpuem.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gvgdylurq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gvfsztkwq.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gscqmhsuq.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gzeeokord.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gibirddli.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gsvoqyrgn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gzvddvivo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/goqwbosku.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/grhdysmua.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gqxebefkf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gvromphfp.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gwaemhvzi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gmfcqelkm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/garzmkget.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gcsjkazrm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gszjdewmv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gayfbjujl.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gysglayqx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gwhqryukk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gugcdfdrd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gipnbnmox.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gewabhtqe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/guilobcco.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gsdddiibm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gezwfhkhu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/ghuynmgof.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/giesqberm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gilmoydve.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gzelwotfy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gamejngds.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gxqrzhqud.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gretdocuy.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gkqcugwxi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gspzktjaq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/ggouhritc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gevczkfzc.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gglvqjrtw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaxwizjde.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gdjlftmyo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gnqfdnyie.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gacucrydz.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gqjhczvax.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gividigra.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gqcvzjwkd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gglhsxuht.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gphzpzjuo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbtjbcky.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gnimgsaoc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gojldrpxs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/ghahaewqv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gdgvypags.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gttqewnpi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gwfgudxxz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gaiafzuxk.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gbczljejj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gqadiiklm.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gnkixvslz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gxujnoofh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gocdvjpix.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gzvjunvik.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/goofkchem.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gvfuilouz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gkwkyimwe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gpepttqov.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gwdtcaczb.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gzqntkfkz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gqemjnlli.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/grsxleiyl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gygofujwx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gqotihhvf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gkeipivoq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gvxgcfyhx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/giwqnljew.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gtefswxcy.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gskkaxhsp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gabjflpho.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gjwefckcu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gidpzjvfg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gmothhaqg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gmxlsbtgd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gmgjblrzl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/govdnqtla.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/glbexqlqw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gwcwdgrxj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gdvgbxskc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gpsihjlfz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gcqsqnijl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gxjouafzl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gzkprfitg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gfldceesz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gtqbupwen.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gphvnwpav.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/glzuhamvl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gjkuvjohm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gvppxldek.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gbwnfztlp.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gniooaoep.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gbwmmzlyc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gmntbuajl.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gdgavhuzr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gejbnxcby.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gxnxssuqf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gpnoyvuzw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gvavofguy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gfrtkhzwl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/ghapajcqv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gueiwzmca.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gptyrexww.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gdkxmszyw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gjscckvlk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxztyhhgn.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gofjcxhrc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkvmvwjos.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gajwocnmi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gaovfbkwz.sHtML


<!-- 参考信息 -->