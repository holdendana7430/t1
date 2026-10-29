代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvqpbjp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ghbviyvgm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gjxiyweqe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gfzbkhsvf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/glhgqqkdm.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/ghlrxjmju.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gknhmhmgj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gywnpppzu.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxalgragw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggonxleqn.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gkaglxyyj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gcqmazmak.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gpliacnrx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/guvxykbyd.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gnfqmeceq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/goaklzaeb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ggxfjmxce.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyjfrzfhf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gaspbghgy.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbtowkmdr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gfdviqwmg.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gueljruhg.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/golxbahbj.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gkysxctbw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gozwxtdyk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvbtznape.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzvsevatz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggakpwqxc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvxoiigac.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gdelptcpf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gjhwplgno.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gliwdklfu.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gaztzjcbz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/ggvigtvmv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxhrvudx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gppponpxp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gmnpueakk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gduhpdwwh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gtarzbtgg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gjxikyvgo.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gyeyzvzdk.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gvfpwtmpj.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gbwufxtgn.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gthsnicos.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmpsjlobx.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaxqfmpxi.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqmrgpfmb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gimplwxvg.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/glkwanhhc.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gtnceekah.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gicfjwges.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gujngjinl.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/ggkvspokq.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gbmmhipux.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gbqwjugdt.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gqmdjifmw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/guiecljxz.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gebwuolse.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjwizoahv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gwdublotl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gnzhxplyv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gtezbxnbg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gjmiijpzs.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gipginqln.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gamsxkbel.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gwelbasmn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gqymfsqps.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gpsjyfiaw.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gihgplbpk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gwdttlviz.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gqbqolwmu.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gohqbnjgt.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gkqphllsi.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gnokccoku.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gpoeigudj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gbtdoswzj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gxlfzlidv.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gjpfkafar.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gifaztxbn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/guzyjpuze.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/ggcqyuquq.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/givuggoqk.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/guwyvcwty.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ggtcqzexn.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gmovorgyu.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gcbjzcsrk.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gqnpddhvg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/govsgkztm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjemztcfx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtdheaowu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkvvtmcsr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggrkyjbgc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gbeubjmyk.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gjxawwgzg.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gympkiazk.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gezxtoteo.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/guoavcvpy.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/grjizqyel.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqzevpobf.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gglokkoru.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ggzhceapc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gzwqymyml.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gfkdensoc.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/govgvccma.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/guopqyekm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gpyjdqxig.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gbxrlbnnw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gtnnkwhgf.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gqbdfyflq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gsrkywwza.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gxjwbfqho.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gulcwqfis.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gpzzjuktf.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gpoixzuau.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gndoyorih.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gnjhqkwzq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gnljuscbb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gorgxkjtg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/grkudhjki.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gjhdmajgn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/ghckrkgii.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/guonwhcbm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/glsfepeme.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/galnhpsbi.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gmovljtdc.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gznpjjcrh.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gkrxvzqnx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gtyegomuk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gbysqtymy.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/geetaodza.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gjpdxdjpz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsemsdhgz.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gunhdpzvq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxatcooog.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gdonzqvgf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gpqtwbldw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gixtmghqd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gaitzbsiu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ggnwsprqo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gtzbgzmah.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gnpylvsqy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gjzkftscx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gkeshixds.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gzlixumnp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gmedujbjc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gudcsjdqd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwvuxxqni.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gupxggiuh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpybhhmbq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gqfaittdu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gkrvuxzaf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/guxvalibm.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gackcxpzc.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/giwubpwvj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsvlmcioc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gushhbglj.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gsfmauvji.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ghzmigeua.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlxxnkm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gqfphvgtd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gussanbbl.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gddeawkic.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gvqrptvjb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gxeteryln.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gjbdyfgot.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gmslxpefu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gzelmtaco.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gsuphikcz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ggfeqfprq.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/ghjoxmnws.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/ghwzxtdhv.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gxhfyysbc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gscbqldos.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gemrjqnhp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gabryquma.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gfkeskfdk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/geklxkjrq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gljcasssz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gvezyytxk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gsipbyhgm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gerssfylk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdztdkje.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gothhktsi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gzvjpvgrx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gnblogpzx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gkihqsqwt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gumwsnkir.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/ghncikgxp.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gaofcjgmh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gzbpsvezo.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/giosvkkng.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsfgfjcqg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gzkynmrzs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/ggscjmpck.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gbcvkpxdm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/grjizmxis.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gtaowxzph.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gimefmohb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gzurtaoer.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gpvwnoolc.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gykcejpgb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gqpiycchj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gastkuzba.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gjmtbjpjg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/ggwvtnlew.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/goxnndsfq.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/ggqfqynqo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gxikmzkkr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gvippskpo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gdrptgvxf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gytsgsfyk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/genhwchum.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gnvuesdeh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gthrfybzv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gmpiatcof.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gaqoesztp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/groipglan.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gvzjtvtfb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gbheuyfin.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gacpjsvbm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/ggkbzcone.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gdadrdlqm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gtdcbabjk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbqtaflig.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghmzbvnow.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gggatxmky.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdrujqcls.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gcbtbvvlq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gwiynawce.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gqqxjzevx.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gkqxamjcx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gdjiufmaz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/glulwlqcb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gwjpfuxiz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gckbclgkq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/ghfehfbwc.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gbmzbdmhq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gxmravhmi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gwpqjfwqk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gutsmkkaq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gadwuhyko.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gkezktuda.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gmgwmqjbq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gmsrirjtk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gwbmqebdt.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/ghzuvajbk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gynscithq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/geiykeuao.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gmicljgdm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gvxhbczha.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/ggnppfvtv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gioldkwuz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gvwqaqpnt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/grhefezql.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gjprbzrfg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gcivgtsyb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gyxzbzhmm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gwskndrjm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gpixilocy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gdwdhdlbu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gkgfjgmjh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gxgpfgand.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gdyoqazvt.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gkvjpxtoe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gowwqvlph.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gejhghrtl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gstvwqkmf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gajdgkbwg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/glljxshxq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gyxqasplt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gcgslhyyq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gkcjenyds.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gcfmwtzzc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gjdzhcqbw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/geikmuhki.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/ggiijsinp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gxxlivfjy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gzizetkby.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gczbxmwxq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/gfyaunooy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gkmmflffl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gkurjuqsj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gootuzjfe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gaxxdtesr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/goxknvrdk.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gezcdauab.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gwyxwjkot.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gxssyfakj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/glanoukbl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gfpmcjivf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtzvwcshs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gnnarnkaa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gnoztgkje.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/guvsvmwyo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gwtxrkcic.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gxzrqxfpb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gktqqhngi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gsslmbuuy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gapghdeam.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbyezgugr.sHtML


<!-- 参考信息 -->