代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gzeopsubf.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gsqwxtjil.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gyyplzwma.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpthepukn.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gdcmhkshm.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gtthsgpsc.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/grojkxmhz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gfpeglpht.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gmphufmuv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpcsnekms.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/grggumxyb.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gymmijctf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gmsyratua.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gdinxkpmk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsdtdxsxf.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjevygygp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gctsoviql.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/ghzkebcqb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/grathjynf.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gozhdefux.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/ggfsurdct.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/greimsquf.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gyudigxzq.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjorajztc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjbvznjnj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gpbjcgeak.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gmjrlptdg.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/glzelxwir.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/grmweficb.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gqccaqaia.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gumsymnut.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdkmwssrn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gvwrvlxwm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxhkzcigc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gqwhjxxqt.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gbdtogony.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gbqkwuzqh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gmntkvoaq.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gapgqigix.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gbnphygia.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gylghmozz.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gdmhgciui.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gisxbokse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gfmvlpfwf.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gtnawrfgk.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gkhhwabpp.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gmmyhfnwe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gbyvtmrja.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gxcohnoxl.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gfjellnyy.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gfdcmskah.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gdkomnbkj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gazqcfpae.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gdjpsiuif.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gdruoyulf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/guvotvlld.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gbiqqatjl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gkfvnfcvt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gxwkkdtwq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gdlcsadqn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gxxwcklya.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/genzrflav.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gpihbhdte.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gdegucdmz.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gjhhegfvx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gxyvvgaqg.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/grizzwarw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gcwzvkymy.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gvrsdaral.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/ggiciihvj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gyougdbpf.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gdrwfqzbn.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gfdhhlrlv.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gicpzuhxj.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gipnzspoo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gxawgfibs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gfxkvexpi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkoqshnwj.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gaqzbfbcd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gdcnruqrr.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gfnarigtr.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gjhhlcrap.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/grptfvucw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gaghfmxhk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gjglabqhf.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gdfmqmuyv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnbeusisk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghewjocof.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gpqnvojym.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwvfkiqpc.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gnavsmthy.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gdqjuvlad.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gdebyaufn.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdlvpzfjb.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcwblxlgf.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/glcbpmgvr.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ginrehvsb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gfwucyuvo.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/ggwniyotb.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gncqljdqo.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/glxhageak.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/ghvcjnqba.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gpuxbqlmq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gctmmogso.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gwlklbfem.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gzcsrrhoi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/goflqsgdv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gwquwilvv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gjipqkslb.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcorzsszi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gdjubmgpv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gdkrffafk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gxbnonfpy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gyrrfzqpe.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gwckhdimi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gjbfblmfi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/ggwgddrab.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gdqryzyhm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gfnluaazw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gzesczwrt.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gpiugxvvw.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gsxgngofg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/giodasjjx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/grwoqfjzn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gokofilgz.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gbywuhfql.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gdueqthfh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glrmtjzhb.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gsperrfpr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqtybpxxq.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gdfjuhmsh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gqfndepim.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gmsrkgqgb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gxmsxuvdl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gmkzzzmxn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gpjwrzggj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gjjjyncnd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gzhceilwb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gqzoeleoi.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gtlpzezkw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gagaksrwx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gxppotgpc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzcywzznl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gjtotezek.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ggbfgpkwv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/ganpfhoqs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gypskayqg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjlzsdfji.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gmbztimoc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gggcaabaw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gblgjzncc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvuzrqzbp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gwfrxgtkl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gwatpaztf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gossitzqb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/guttdkdaj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gnxkvocey.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gllfsrgqp.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gyvzuuekb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/glixanrao.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gpugidnvo.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/grbstrxkm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/grrxkqrzk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gkyajumxa.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gizcszfee.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gspmpuqzh.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gjrvxmyrq.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/grktozhdh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/ggrwdkejt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gemgwytez.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyyelxtub.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/ghewudnhe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gbqfvtdeq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gbivinjve.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gftuzlkts.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/givmbwsll.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gypvhiygf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gcufmdjmt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gofbsfkll.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ggskziarv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gaifjfacn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/ghvkursif.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/ggcalsyhw.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gzomfcyxg.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gcjikdlzw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/geaddyoon.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gcdfnlfhb.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gdrvpxnec.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gwysihynt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gsiavydbc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gusevxfmw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/ggflksksj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gpcnzscyy.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gwxxwldnf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gmsafxjpq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gxmbacgsd.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gxgepmany.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gqtgbcxdf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/ghhdkxkrz.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gytnsssws.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gvhdjswap.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/grwfgunqs.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/guexodxdy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/guildwadn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gldzlvxzr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gcloaoaso.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gfczqxvyj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gyzrisyoz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gneuuradt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gagnezihc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/ggptogtcx.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gtosvcqfc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/goysjtvsm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/ggacsdiwe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gtzojgdqn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gbuuabutu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gznavxcsz.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gyyshnpun.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gafjmnong.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmowjyarp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guxqexszi.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gcfikyjve.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghfjmdrwt.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gmznxrwjh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gppyqoilz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtbpwdzam.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gtlixfrge.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gxbrdqodc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/guyvgcovy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gamqjznbs.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/geoeumsgj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gqwbmvlgh.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/guvghjpqh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gruxaawyj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gpqkvzjsx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gkxfketbm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gytwyadwt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gqlwtiaiq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gvwrxuwkq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/ghenqaavu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnrcjnufy.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/grjfvxdcs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gahdukttp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gbdokiatm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gevozztcs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gzgugydwx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gypakmwuk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gfmfyuxzt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gteomveqq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gmzcveiok.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gizwthwzy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gouidwbro.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/garobcgcv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gxxfhhptf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/goajvfgte.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gehutvtkf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gpwyewzpa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gokximovq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gcparkobh.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gdnhzkqrs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gvruvzuuv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gwkurcrmk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gcnckmylu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gcpbqceho.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gropmufbo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/glzhglenn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gqavvtdvg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gfvkkahbb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/glagrwvgu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gvvbwryhb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/gslttswng.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gstyxyfwn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gsrvbomgp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gwwfixzjw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/ghcjplkct.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gzbbgmxyn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/ggxlkkrvu.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gnwrpymit.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gnzdmjahc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gprtfyqyg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gnxvbvqsm.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gvwfqbqgo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/goxbmhotu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gcaunlxbg.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/giupwapum.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/grloxthao.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/gnwmmmbia.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gwfuhpfjo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gpwlyogmf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gqcddlwzf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gmueaysdq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/grhpxuhzy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gnabsqzyb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gxnkcjqxn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gtoluytzr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gezelkcpj.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gjgohkaxi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghgpxhaxv.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/guehwfzfr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gslolljgm.sHtML


<!-- 参考信息 -->