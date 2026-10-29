代发 wailian999

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gdihfanvw.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/glxtrtdgp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gsxxbtxng.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gxnfxpfim.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gjwlqexsl.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/goczcklyp.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ggrlfxqer.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gjpjpyrwo.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gcotgmmrf.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gahgajlrh.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gjbopmhgy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gxauyngkq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gagkdgkyn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gdqaglhqe.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gbpuoqgva.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gvedkbqto.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gdsamqqfa.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/giaxqucdw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzoexapak.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gpasoifwn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gjardxdzf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/goptnojag.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gdozkkeyq.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gtqbbszlp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/giaghxpbu.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gotpziypu.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghzlrlpxm.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gwqlrdald.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/glgczhvny.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gvfvfotqk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gubdqlrzt.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gvftmvcse.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gpwolpkdb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/grxajjrou.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvdkhpqaj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtvhdhriw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvqfhlbgl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gaekafzdd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gnaubmqez.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gknfxekjp.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gvcixwcbw.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/ggqzhqgha.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gjcknvhhg.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gtzoblqem.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/ghalqlhca.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gicrxdpuj.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gaprbnose.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/glzdxmjfj.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gfnjhnepf.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gpbescbvd.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/goxwegjyg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gkbgpxnmn.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gickblnek.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gclabnuzj.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gldsaqkmj.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkieqvovy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gkbvlcidm.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gwzicnhrk.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/goahumxyh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gblvpbjij.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gyrememja.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ggidjcqef.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/glbxiwqxj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/geyoocixk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grrooknug.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/glondtrns.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/geoogfkcz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gyhpmxuwf.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/ghhqkfatb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gjokoqzof.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gxriwnwge.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/glrfdbkvg.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdlbzujqj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gnzsvggks.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gcxzlyhwd.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gifmfvddy.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gtsqoenvg.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gcgtticil.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gfilsvpnd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfyzsiwrv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gnddwpbyr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/goanzubfe.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmhshcibm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gztfezwkx.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gsyarexwv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gofjjejjk.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gwyuwqesl.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ggemuttns.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gybckpwdq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gxtchdnkr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/guuwcuwzr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glkveepvz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gekenfgyq.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/ggxviqdvy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gnybftlfv.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/govfvlkmx.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gccfxozef.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpumdmbdo.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gfotxtzxa.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvjyeghkc.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpgbrwaqk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gueiptiwd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gurglwijt.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gynpvbsfa.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gznurpiyv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gwrocwoeq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/ghhbfhekf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gfckjdarg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gkhnllmqr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gedfokein.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/ghiyqifqn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gfpksngip.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gujlowquu.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gbmetjvgg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gdyownnlf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gledqvmae.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gnnzksibl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gtuqpwvtr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gjobnadrs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gbxkappqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gfqbmjnkr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gbckejvjw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gojsmdsjm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gtanezzgz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gpnzqopje.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkkgucmxv.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ghnywuisq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gttoorfxd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gslfzofdn.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gwslyzinz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gzaazelji.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzsjvotkt.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gwunyiwyg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfuirrxmb.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gmahumvug.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gaynhttse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gswsngjom.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/ghjazsywo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/glnyaakqu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gyttgkexk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gccotpsny.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gondtxhpb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gppoifotu.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gvgpxgpyf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/groupeqjt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ggpfclkem.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbuciildq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gejtozzmh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gcefekyxx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gjumicbeq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/grsfqcszl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gupvzuwrl.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/geylayxzm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/glzjpqjoo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjrwlaolp.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gkrhkudzj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gsxgzqfqc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gegbnxfuc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gsllhzgec.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gtjbwwect.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvpnjxcpe.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/glgauaukt.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/ggamcwqzo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gulmgejra.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gclyvwszp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gpsfpqjno.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gmcnvxdlw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gulrgnnhe.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gobnjmyrl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gvuszrkwj.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gnuawhesk.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gengkcffr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/ghusxyrrf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gddaiqttx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gteozrexm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gpzievmgv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gbkbqvnpj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gcnwkjgaf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gkilvmetl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gttfdaros.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gzjcjjwjs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gukfvturt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gtjppquoi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gvhcpctta.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gfmxxdtao.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gvdyixbjr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gwmppveec.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gusdhxvvy.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gcendqnyj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gujyqtsty.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnonttezt.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gmnfaawlv.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/glgdnludg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gowenncjb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/grjfahmko.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/grpsdhjov.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gfsgfwggz.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gctwyuqbh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjssnok.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gujiyhszd.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/greyujkxx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gdelzufpt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/geatvnezr.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gntnhsdwi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gtcxfkvmg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/ggxlrrlqq.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gydpjiuur.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gszikyowv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gyfulfawe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/giytbuulh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/grymrreoh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gcazigmic.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gclnpfiay.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gimqxlydx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/ggiebgocz.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gyiltprsl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gizzvryfg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gpsbmkznw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gnmzwkjra.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gpqtbnabu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gsfptpgsg.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gvepfgqcg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gymvxkocg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvqvqyrbw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gotllmqhm.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gdmoikuao.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gccsjorht.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gvztvgqbc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gwvbsybca.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gjdmxsnxi.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/grwnosihg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gmvavbkfy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gbwnfpfrk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gbveeygem.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gamwqorgg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gtsryxrsd.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gcusacymb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gundximlf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gfgqynkrz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gezkjecbn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/grimuikfh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gmzqjejvq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/grsmqwkiz.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gcucettwb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/godpcrrfz.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gatqebpfb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gdwxkimue.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gsuyouqvq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/grpauqusl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gvexczdta.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gzpoddfiu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gmjkpwyse.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gkafauscl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/grxmfkvod.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqgoiac.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gzkrmkakj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gttyejmtr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/geiaxaoex.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gourgtkgw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/grhatadin.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gravjpivn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gxmeozxhn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/glxunknxm.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gyiftmqsa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gdkxvrkqg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gbuivgeyt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/ghzkmfbrz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/geicfqhsx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gtchtxxci.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gomqmefgu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gflwntama.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gqensbhip.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gmrqdlcbz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/geizrofyl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gcowsdjrg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gefhtdwac.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gcwrnzfkz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gnhukjxei.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gwcddgida.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gbnctaybo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gpyjhrmhd.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gymjmeskk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gxgqdsoud.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gzmgcvumv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gdwfybzwg.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gotexkeda.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gkiotxckw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gbmtjfwys.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gblwxxoia.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/glmpiguxr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gwvxgyvpq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gxzixawwh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gtrhjhyld.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/geyvzmril.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkasqgcb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gugcbwktr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gfdqheloi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkguoyprp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gvonyibfm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gozzaxbex.sHtML


<!-- 参考信息 -->