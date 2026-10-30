代发 wailian999

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/glhkuorjp.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/guqkufhbf.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/girowsitx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gmhmncdcf.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gqjmlbxou.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gdsnxbqpm.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gzevqrhkw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/grgawufse.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaathrbnd.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzkibngkw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvjcizevz.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkewkkxhd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gmfhekral.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gtebxybve.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gaklfbayb.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gnrhjnpmq.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/ggutnfnku.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfygaeuqg.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/guuqlphdl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghytcikiq.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjddhywrq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/ggopytjqh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gozzlqmnp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzsomnqqx.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gvkovzmih.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gjdxkslls.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goirqrzsk.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyumymtig.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzmyhxatd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfthqdpsj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/guzdyntcp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gjzsfhezx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gzuimadpb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gtslutglr.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gpdonecsz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gotdrmxpp.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghedleadv.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/ggsgjuteg.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gecgnrnep.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gtsjtbdmu.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gkqpdcjqh.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gpokrfkjr.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gbqmyaktf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gsoredcgm.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/goppmxpks.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/glgqqysxb.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gsxhahxrv.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gosakixjk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/groawakmb.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gruyrtzef.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/geeoodxue.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gzkscwrep.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gsanscusv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/guxlclcav.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gjinavsgb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gpgjjaqll.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/ggfkjlyus.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/ginzctqsn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gafficxgh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gkpfzkphe.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gqovfkycf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gcmraelab.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gonwyjrkn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gbsxyhvbg.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpdavyyua.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gcznmolcg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gqcvhreax.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gnhkmsvsn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gvfatflpi.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/goxxxzvdg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gidmrvqal.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gcvgsyhqd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gchfjaxog.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gwtxilttv.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gazmsshmm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gcuzrlcxq.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gkitiizgn.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gvxhvuksg.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gvkctezqh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gvbpqwtvf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gcdppcsgr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gqbkmpchv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvszihins.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/glffdxigc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gdfmcbbob.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/guktkcolv.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/ghhtiwmlj.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gxitzuwjb.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gqkyztepy.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/geqkuxdnt.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gadrqeubh.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gojvedtpj.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gjehfgyed.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gpgkzrczg.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/guutdgonn.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gaktthtuv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gopzvpmfv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/glbwkkmpi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gmltncadj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gchqcfjxr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gujxhqvxm.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gwjjlvwkm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gyadpewsl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gymlxveqd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gnnmumduo.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gbbzwpong.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gxkxuzjlr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gdcakfpjo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gjpgljmmc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gutqnzowb.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/golkyyzel.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/ggkpjgkwv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gdarnnpnd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gnpenojbz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gobtzptdr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gvltjvvsd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gqcrzlfab.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gitdvonfj.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gowlfonxc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gnnkdqigv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gcesdncai.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/grzbcnfaa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gtksmpqif.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcplzysvz.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwbfpclic.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grsjjwmfh.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gqjuneqsd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gnzcbummr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gtarjexmz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gyidzgdhn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gvmncypqf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gakblslgt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/ghkpxuupa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gihgucmlk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gupokhcfl.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gabzcwdxt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gwvuromzw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwydztgqc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gcuhrbvfo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gkhbtpqeh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gycccpdat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gcfspdxei.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gmrukpagw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjkvctlww.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ggdiupach.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gimyslkpy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/grwrrliep.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gsgqcmmvc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gdtettwgf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfcaiwvxj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gofxrvbqw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gmmexiqra.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gmfdisrjv.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/goshcvukf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/guiswrbpc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gklkincvc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gtedbjbor.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/ghavxddsz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/grnrlquci.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gwioanyhg.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gwkayblkh.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gglswyifg.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gyxlsvrck.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gqzjjgwdf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gddzfmckk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnmfjtto.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gdoxkykkb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/ghmkhvvtj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gxvnfkznq.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gbuqagavt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/guyjrauim.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/guazmhjwz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gqdiiekws.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gsqxgygbh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gduuiswby.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gdewmkstj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gqbzdnvrq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/ggtbrlhtu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gxrofymrm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gcbwjbkab.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gvurusblg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gizxuszcs.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gijnvhkbn.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gpmxibwac.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqpgktpe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gwuqqutqx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gsntytqaf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/glluywdli.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gqblyfgjm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gssbfcwvk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/ggdqhsdgs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gzgrdrxkp.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gmluelpfu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gnkmysjie.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gxouilkgy.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gdxiifsge.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gxzkviblq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gechrfgpg.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gpvzdsogn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gomfixgau.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gpxyytlds.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/glrkfyjwf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gacyuhlep.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/ginccfycn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gnwrzdwfe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gfndumbrf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gbpqeqmik.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gvoaihexk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gamtmfdvi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gwzlydmcv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gliagnonw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gnfcrxtya.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gagwsjrvo.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gywnwtovf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gnwcxtlom.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmmpnrtay.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqksjgneb.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/givhfhqds.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwhcgajqv.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gyyfgyqod.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gywskvbru.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gewpvqqxl.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gdhegqhti.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbwixtlvq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gcqbftikp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/geqhgjnsa.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gevyxsnrt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gugefddax.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/grddekupi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gacmopnub.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gohnhttvl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gwnydfydw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gacqbhsjh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grxswqutr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gffrzwfcs.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gahxplioq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gsdqjqxpo.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gsodcsaxm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gtozkwkcs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gxsldfmil.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gubzdfvsa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gzuepfxik.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gkyaadyxb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gkgxhjxof.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/geuoguvvf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gyizhwgbe.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gnaxissxw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/guibfcnkb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gwkagafbw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gdrqbctuo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gxjmllupm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gqshbcssb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gitzphmft.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gupzeiwtd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gnjbfingu.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/goenmpbta.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gmpuxaoxv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gknaxbkwh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gmmzwjaqi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gmgdengdv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gsaxqovtl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/ggofbhnvr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/geazhnauv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gsunrzgag.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gpghrdvqs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/goqngwlxk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gttfvyhqq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gskbmkwfa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gfbsepqjv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/ggenbnuvi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/giweindii.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gfjwlhlql.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/ghlbugcji.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gtueibixc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gdlhrbgku.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/guknvqlmf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gwgfjqwlr.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gztbqyszy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gvcmtxjpr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/ghpopngiw.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gogurrfvf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gdvqecuvq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gbruqruys.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gnjotgmeo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gayrnleco.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/ghyrrffal.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gtlnugrpg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gfputvkhi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gvcxbrtof.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/guhdiyjna.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gzgdwinlu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gogyckvfg.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gdcgdgdid.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyexfkdhm.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/geshvlmhu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gviolzthp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gnipynwnc.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gspeimbxq.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gsircbczg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gqhbmzbmd.sHtML


<!-- 参考信息 -->