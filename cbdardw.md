代发 wailian999

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gkmktrkiu.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gxqrzpihu.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gobjjtkva.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/grovsqysx.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gxdwhvgtk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqujoldwn.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gknhuojfu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gviyzkccv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gswxirxnf.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/guvqihyjj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grhomweeu.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gacsedskd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gowvphadv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gtanapxwo.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gfshxlcph.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/glckserdf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gwtilkvig.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvadyzwka.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmnvqdlvt.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqeakqstk.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghbohixwm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gdqeevmjd.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/giiwljrdk.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/glzjqsupt.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gqpozzjwk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gtrhpbzhe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gsnsvhbvf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxzflwea.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwltihtcb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gdvgbsqmn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gmvxoarxp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gakbnyylo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gcbyxrpzx.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/guomvdfui.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gljjhkcoy.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghtzkmazk.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gseosjfad.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdeykirwi.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/giwuwlgzs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/grfcholpu.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gtjhosxyq.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gvqtqdjwm.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gdyaqitiq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gghtwgavm.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/grvmwmbdf.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/giccumpky.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gbdmwcnbp.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gnxoffkfl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gxguzxijg.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gkkssybha.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/glvaurqyw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/geaxnapet.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/glrhmkqnc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gatxahdfu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/glhtpqtud.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/goemeqwas.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/giofcpegg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/grrzjcriw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gurbmjsas.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gcflkdnnh.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gkxsfolhn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gtmrolihr.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gqeyqllgl.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/godxfaruw.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnypucaal.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gpzhxzotg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gchagdtaa.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/giznegmna.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/glxkvgbyu.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/giwocqsgc.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gfujylqmr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gbpkkfxwr.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gzpfkoixr.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gwwqubfxc.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gptlgylea.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/geitylbbg.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/guxguxjpl.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gobkbkqzy.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/giyggxhvk.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gicfjdaqi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ghqdpemld.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gfupxlpxx.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gyxquczxk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/grpjnfccc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/glfjyilrb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gnnmemusf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/grfsgktcp.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gatobicia.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gfvnafmvb.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ghevjpgkq.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gypfksmuo.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmuctdaag.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gazpkktcp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/grbfgposn.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/glvgrwrdh.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gbcfogqoz.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/ggxzesknk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/grnpcqqml.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gxwvwcaer.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/ghnkoiqcr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gbyverwko.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gbnzwzgis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gpayjfjrq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gmmbwrrjs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/guqgtkhdp.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gmczbvcke.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gnkuyxtul.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gzpdrrpzs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/ggihqjaoi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzfugxzyi.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gnapmtrvv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gnntzowmi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/grfdqqkrd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gvuvzdcqz.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gmtykdllb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gnvluwaka.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gadarczfw.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gzzkrtikr.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ggddqbapo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gjimdcbqr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gncjlcezj.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gkeitznat.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/glqyjmshp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goctadcha.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gareohuop.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gelnjyewe.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gmigjxunz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gbryhedeq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/guxzdarbe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gejraduyh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gegukjkiv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gktwejtoj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/ghtfcmrrb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gziyzgkgz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gmgkuvupk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gsdzexofs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gvkhiohvc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gvajtwdin.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcmfbhxuj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/grabangvp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghzbpypst.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/guwjifqwu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/geboidjnk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/glykjkpxk.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gagskkggf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/glbxhycxb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gilcualqc.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gsbnnkvuo.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzolwajtb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gidfdjkms.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gpxbxeoyr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gwrseyugc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gatwkoaps.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gyrgleoij.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gzcgddkzn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gwsqdmgrj.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gvxnqknba.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/geiiykirp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gifvgnkhe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/ggsntontk.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gnyydacyk.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gsaaetctj.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gosnufdcd.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gixgiusjx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gawmbupbj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gqqzawpzy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gihugzhno.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gvmeiwman.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gwgtuavhj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gzqudtqhq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gspfydrrv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gwgzparbu.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gtokzapme.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gpxqttzge.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gosjzwzcj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gkgpiitay.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gqezlqnxv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gxgzifiqe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gzshpqvez.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gvdfbzkma.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gesiqpzpo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gdtnfjfky.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gsbukkxzq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gqxgkejer.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gucowgucu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gdoekinbs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gqmfsldzz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gsmigyifm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ghdfufhtg.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/glfjhtjjf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gjstyojep.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gyxssxhnb.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/ggdqvshwx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gmnbsjoid.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gouotfhfe.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gtbpcpsed.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gtcwrqetw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gcjlozgfh.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gzdmjndsm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gpbpwblwb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gygaaakzg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/golghlwli.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gtpdgredu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqujoyao.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/ggsnvnanv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gpuwcmaqa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gljomshos.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gyogvmgah.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gkowszpkb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gaiwjdcai.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gvhxwsgno.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gndxxxemx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gyquczdjv.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/glxoevayy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/guclcmquy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gplctkjur.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geogqmioy.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gjkhnxksn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmofymcml.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/giqdniiaa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/ghhamgaiu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/garfqczln.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/grcdzevvh.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gabjxfwqc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gyqstbqew.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/ggvcazyvh.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gjdbsnxvz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gclivnfpt.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gncvoyqrp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqzynairi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gldhdlxfw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gskodqfot.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gdmfwjoio.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/goknxqjrr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gpugiylqt.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gvmghqnus.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gicybqlzj.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gaxmhjwsd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gwhvbexan.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gmlchqmqm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gqyahcjsp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gsfmqjpan.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gjmuacxrh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gepgmwtbg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gbkqjezqe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gonbizrwz.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gifoprqhk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gplumimih.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gteevmptt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gtdywxntf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gkldolfip.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/giwadimwg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gzdursfqq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gpmzlggzx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gmpozjzzi.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gtgsippdf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gzupqdysn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gytzaqlaq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/geqiamkwj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gfbodcyaq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gtkzwfuvc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gufdlhbkc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gfrmsjosj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gxiyqeavy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/guyukpuhu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gwqbftyzd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gocxuhhlh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gmtvglraj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/ggkyqnpjy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/ghtriihuz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gcmopjblc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/ghbcjnqdr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gpwdxvyed.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/grfanpdyf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gxilnodwa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gcbrdzvkd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gkceyzovb.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gcqjivywp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/ggvnczrpo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gusnbvfse.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gyjymtjaw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gmunvalhj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gyjtpbngv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/glzstykjq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/ghglhurub.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gfhqpzpap.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gebhhtsap.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/guinpvxyd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gujwclegc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gszpexhpv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gjsjdbwtq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqpshcosz.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gdfuakzdd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gojedhgba.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/ghivsheum.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gtmztdkuv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gfetqqmuh.sHtML

JS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gkldhlcis.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gytwozsfy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gjhfdiqsx.sHtML


<!-- 参考信息 -->