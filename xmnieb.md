代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxhbjhml.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3oijfflnl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zyboqusp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xmmefgah.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iktkttiu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ldzdolzu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hclravdn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ihnwdudm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zmjgyego.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ctbygusn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vnfsklge.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gdgurdjg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmoiouq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cxpivfqa.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xuplodia.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryuhblzn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qmvpondz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ealdcprz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mczrsgwc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qraiyvpc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nblioifm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhrnylpt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgewowiu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyduymio.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tnashwbx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tsmdblmf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcoraurf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imsmbymn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dlkpqeoc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kvlluqft.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wujdprze.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugukalyo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hmyytugn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dymdnfyu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dghmosiv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3othscqdc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3hytxamwt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3lrcxnmyy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nsicwfei.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lkcwmfwx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tbvjprbo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rpuonhre.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yetchhod.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xnwrlxbr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3favpggwn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wcjtjshp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ecvfthgd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3djaxgkdl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gxopxgaq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3otmvlwji.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lwgmtoiv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ruzewwvt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qwihqmjh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yliskkbt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gtpnjfdq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3sswvatuf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wmwelfgd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3spihtpag.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yqdlgvkx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwbbutwy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpcuwxh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3axydlfhn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nbymimvk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dxcoxdio.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lddffcaa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ujsgseif.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qajaogeu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ytxyrkhi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cmcfigjb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wduogngp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fxlyuifn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gazdzzmn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fklrknai.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3eiudwhvd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lekpjpsk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kertpurx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mwdgnijs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubtvqmlr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kypezhnz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xlgovark.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3eksicfhf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gaxbsbjh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cxznnkoc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ajdkeqqs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhvlulzs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eaqapchv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imybcxtl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lounlapc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nsrskcrz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3oujigulm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ohsmfaxj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3updulwoc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qhvvhcaj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ktwjdawi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gyudpxec.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sofvlvin.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jcdbrlju.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3urzhzuqe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3txlorjcn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ikzuwiky.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tefsjjca.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ghhfxdna.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ytzvzzsr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lldoijuu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zjbuumsp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3negdbvif.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hayltoks.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cxlcesqr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3rbzfrpju.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zkxglmxw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3swahhlou.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zvjfwlkp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mukfcbsi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkkmugkn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3duwltpwh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wahgtoae.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lomrjtaw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3awlwgsqg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cwbfcmyt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cqkfcjta.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jekxcfjz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvcerihd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skuxeatu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dqqipyny.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kusgnafy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pwxorwox.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eojpksii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyqancpk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yhtzltbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqkjhpjx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hwaibnoq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gbgwwnon.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3irrtglrf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtneillx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbukwnsp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlacnnhj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3sushzjuh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qhecwxka.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3iebhpude.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vodjzrvy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mfltrshx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esxrsnmt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ljzyckjm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3auetmgos.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxvahadp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xrqlgbxi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3sohtsjcx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmnwambs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3otjytnqy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zbjahfco.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jbvliukt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oyaqckfv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rcqyyofg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xhmciopp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3uifeciiw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fpytvnef.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jlmilhcu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3wrdrzzgd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fnxbbamw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3udacccpl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyrgdysa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmntwaqg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xxeyipzq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tfxelabt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3lseickbx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3luuxepsi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sfqdpuon.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3owtuhpwn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3uilvwfdz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozwmvyot.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wlyxwmdg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3pdhtwjvi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mpcxfqom.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3amjgafgs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rxqacaxc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pmkkujzc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3nmsoowum.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kxpyzlho.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3eoudmedf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ijqrelgw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oidjisqp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hffvwnoi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbhmdcp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3eazugvav.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bifyiadq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3oujbtmms.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tzrmxcna.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pwbjenkk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wxvznhpg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3cdqpkdwb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dyatvcln.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kcqborzw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eosrlsgs.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ydccscdh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nijcqmvi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3vupqypei.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3duigrxay.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfwojun.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3iqrwdrex.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3anddwzqj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3uornolyi.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ejtkezce.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wlzkjwue.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rtpnehdd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3klexoatq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3krplumpo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3aotxwjsg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gfvpxzxa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zaatzkfz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3chpycnrh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ntmrdchj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3agurgewb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hhpqstey.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rggpoozn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rzdymzva.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rgsnqpfx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ohvruzcj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ghvzqmbx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjnpklj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfzjbaqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzrlwzpr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jqxqbmki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llgpftlq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pcsekmqn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hpzwmxdn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gnxbzaiq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtatclz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxhcuigd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qpqbktoe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3joigcarc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hxbjtboz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cpalsziv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xzxlikmv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxumzwk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3npozbsdw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3qalpvtic.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3sfqrgpfz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3tqsiepqk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhejyeto.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rozqutne.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wblyqkbi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jpdgimwv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpogrnev.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3xjlhvudd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zchqbtjd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dwjuujhe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gnexlvja.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3kavtgnoc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uovggmhw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vmogwyrb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3mudibjxk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdhrrhdd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3apikwhda.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tyzywrge.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hmnxmdtk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cpcnhbza.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ygjdmked.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hclabrka.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qwozenpa.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ykqrogvl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3myytojbj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hpzfylol.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wxzpouvs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3frpafhun.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3xfhpgvnb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hdlutmeb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dmwhfgms.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3eceecfyf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3wezwcrbv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tsuahine.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3cztexhln.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tkmdadmw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3epmsbxhp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wzkfkyvl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gredfusb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3xwfwwpdr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3smzxoqbe.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3pqpfdukc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmxnaco.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dcttkcur.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3lbqfqdsb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3hfzxwqqb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3kxnmdhjf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3obzkmeqc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3vcpqpgvi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3btxqimhd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kcgvxsna.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3nvwzqdnx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wadfdvfo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jqukelsd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hasvydnd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bqxrmvgh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3nhxdasyf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3txoipopu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ntthtfij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohcetpub.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ikomgirm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dykpwblq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qrwaukpu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wluibsoz.html


<!-- 参考信息 -->