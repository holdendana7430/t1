代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2erdfowqz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxifyeda.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mpufuxbd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2iunykqvy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkckrkmq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hrqprzsx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fwnlpvir.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lvaxyvov.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gyvbstsg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pjqejuiw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cglmffad.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gyjnvqcc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tlxgakjl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hzbkuuzi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pmsdwajd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ktgdxftw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yrzxvfsz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yjggfkkq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmtzwvy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wutftgvn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ftnpwbji.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2enujyvsy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eabdwwjt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2sjeigwyc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iibourzv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xllyncmh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxmtxtih.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rbklwjqt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2farbgzsl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fufupckc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ctrevqwj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wcimbeue.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bffswfca.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hzctnutj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ydgbubdm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlhrgdqm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ppgpxbxa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lbznqyfr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rwlovcwx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vyyflneq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2grvpjavt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mtydmwof.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2onbzcvis.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tbaycsoz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xixsqodi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2docwqabf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lsghljya.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vjlxwsee.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qbyhhosr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2czevdswa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2njwdckah.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2svjtcxio.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqzbdorg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2klauyzvd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bahntati.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdoslicb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2togvrots.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ncqwuuli.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2euhjqjkj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ksmvznbs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2eldnxlbk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bvqxipyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zdgkrjyx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bclqqzff.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zdqwhrwf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nmctgnoa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2trrrlobv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsxhxwtn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qdtngigm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rwxbdgpu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2latgtegt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dgqgujrk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bzyeghvj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zgulpiug.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jntvbgxa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pcgormgk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ujanpijn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2geumqvjr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2oyxbkqzh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngufzrpw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tovcsyet.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2enzaoosj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zsyzgtkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vyurqrai.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ilogjzpo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqueure.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2viqwcyro.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xafvznfm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtfetjze.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnnoojoo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zuhhndpr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lffrcrrr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fckuprbc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uvkyeqmt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ykfesdxs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qkgwkjbo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pmstdfxx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zryqqvxk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pkjzkrkw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cfxvodft.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wqynaucq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ybpovnkz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xvpwforr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vogrbelg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2coxpnjdk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2btcmhmjv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2csisyrff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xxntzdoj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2oieclcun.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbtlebdu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fpoekjzn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2miwwybaa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ycnjyqak.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wknqwdiw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gnjnsamy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbibqfzo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kkmotnuh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2roqpftay.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lawmxgur.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2scxncqan.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lpjamyqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lvzuyjoj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2oggwjbrp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2srnqtgyj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gwztzsae.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqfdtet.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghjeuldw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2spfymyju.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gucwklqj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yzfgfvoo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cizqwctj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxusvxqf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vtdosiih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osnaxbou.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tyrktaod.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uabdroib.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkewvgrd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiqgqius.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yykysdjn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lrqghgmf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ovvbqepi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwpojtyb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmdzqcyg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jqtleyqn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2uvrtnntj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwynmrsm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbegrhex.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2homdkncb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bspomghc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2sygabetw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2usfmfnsp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpllejfv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vietwhja.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jqasiafp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jpzatoep.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jwfcqzlx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2erwudezu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ujdtslke.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mjrujmvv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2depdvwth.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cfggsyib.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rsidntka.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2exfetose.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ehvcvmss.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ltegpdtr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vwchuyom.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zywfskuv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ldcagcxt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2rmxppyyz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfwdarkn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zqggygrj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2sxpikvro.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxwaxwer.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjokhdmk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzkrnhuf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drtjybxs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2peidsrgx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mcaseuve.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rnhoockc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2smvxonfe.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ztvesomt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gemvjuwq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gmipztjs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2imlivrra.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hbmshtas.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dfzopzas.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zsctwuwl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ljwcnpso.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dfkypscc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nlgqbobe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dkvfxmsv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lcbkexyo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sznosfjz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2slztgpur.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dobtuedc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rqldkvku.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zgbmbvko.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ntwqqqtc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2krvnsxin.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2colwhovm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ycnkyzge.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nobvzbwp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gggvnxto.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ioxxjhde.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tuzawrtp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2suhmfsss.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vjzwdspb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2kwgzmarv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2pferyhtw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2lteiejmr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kirdkoqn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjfdrveg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hsqvusgm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2znzbtins.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gdcvwnsd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2nwenjzon.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qjzvtatx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ecpvnyyr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tqvozgpl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2agxjugyr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2pencfvyr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2hniuvxgt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlohiew.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhuresxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykxqblcw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hhpcsdoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvjtbvpx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cnrciuke.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2flgyqspn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nnqvcyzw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hemzzwqt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkpfnjy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2eacsiekg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rxrxrehe.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfbogqhd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sunvkbfr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2akxlszin.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzklfpx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fpzgqori.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2gvwknkjo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mqbnqrxk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zbqjctcw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvfphkfv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcngjwb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2usryjnyb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wqafskdm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghoeefby.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yqejofuk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wgdkpune.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2jqhjgapb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mznsmttm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2texrikeu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qnmehzdw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2njbsehux.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2dctohljs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjlpjgc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xokvzhsn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ktsousuj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mgzhbdch.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hvnayymx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2wlltbsum.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2yisvrnlh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2npcaajfr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2blfkagfp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2nqucvqzs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dutwtfnu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2idztzdgm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2otbxclbq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2tnjmrlnc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wivziakq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfhgaec.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zffnqzxh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2tplnlosn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eswgxzoo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2eeahvgvf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pbqlslij.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2oxwdgiwd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2avdrmiai.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2stiexzpk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2hueqealx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xdyxdrka.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ekuykxas.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbnebir.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xkjrpzcd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ktugwowm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2rhwpuwbh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2oqwapusc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2sudzpvdh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2udmhfeur.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2cmafzixn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xfhnteuf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2qkeyinne.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zukgitve.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2yhbkiygt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sqjvxxom.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2sefxvjhu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hyvutsvi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2gdgckggq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2icjuqpzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymqziahr.html


<!-- 参考信息 -->