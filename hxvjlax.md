代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gegcevkzm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpvmhqcqv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gbhcdhngt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gtbnzwova.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjlkbnktl.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gtkxalraq.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gaqhrbnoz.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/glodciyqe.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gnspbsaoa.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gsmoxooyl.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gpzyxxoym.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gfugqlnmr.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gfrvtkayu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/grbwafkad.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gqieqosle.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gcymgmxpj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gjbzztexq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwpyuiwkq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbbhcdrqu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxajfeljn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqonytaol.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gbulmgcse.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gmduzjjmf.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gzooldald.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gggaxtsqe.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gburrgiyy.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gxhjovcwb.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gdjyludqp.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glpkwbgng.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gthmbeoqc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gvrdzcore.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gijvlliiv.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gojsauvhl.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gukkizqoi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gggnsqgfu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwusrgkzx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gxrqsmxxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gtvmrzkru.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwqmvnmzy.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/guidswxcj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/grzzqjcde.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gdbnwcafj.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gericfijk.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gdvvyoweu.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcunpgojm.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gftcvoqae.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxtyrjamf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gxqmxkihb.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/glpijactk.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gkqclplzk.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gjhkxkqbj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/grphenwes.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gezeixvas.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/guxaznbch.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gqaayfzpm.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gfigxztru.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/guwxytvdo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqyibnszb.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gdsbregdy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/ghumkxlxr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gboaqxykg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gjlmbmkqx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gwnrcajac.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gqqaefxnv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gugexsxgs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/glicypeqi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gnvvucuib.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gokatbvyg.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gzzjjutbm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gcczjzuwl.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gcdxnnexn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/grhbqxfad.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjnorwijv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gglonaqed.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gppvvhvca.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/geixuhizg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gdcmlxkee.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gtcukjvbg.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gnceajstl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gyralqgsk.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gidruccio.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gzpzwcvou.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gxogjvhat.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gwyznlvxj.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gdkxcvxmf.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gpndimzxh.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gjelwchpp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gxxqfmeqv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxmrbohkb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gbquliucg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/goieamtjd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gyazmdaim.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvwxldskl.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gbrxehbpo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gaixbpyrk.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gekyqkoxd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gzbmtlwak.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/ghlhwssne.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggkfvfrdv.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gszffpbgg.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzgxqerqe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/grjaomvtp.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/ggzvqzrhf.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gjnvxtaqc.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gqbqmailg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gmdcmwejj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gbpfrkrxv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gvvjquklb.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gzjchmizz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gwpfczrux.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/growitnzd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gplvblylg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/ghzfgvkge.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gajbucyfq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gngqsarzg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/glbjbenyw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/grsqdjgjx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gfuxpfzwj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gaahnftea.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gnlcfkxzg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/givdclxgf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/guxbosnvk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbzzamv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gxmzlsotx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gkuvcdrno.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmpigycwu.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gwtjocpxy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gajhczbrj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gpdxyzjla.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gzoleushx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbstwtikd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpxnynuzp.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/grnsafcqj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmypjuvtp.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/geuavxwkf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gpamkzupn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gknczyssf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gaelhqxcb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrywniva.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gswclsupe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gdbqnidqf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gwpqpcqxh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gzresqyjp.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gjqewaahx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gqruwteji.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/goqawjjeb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gregbpgaa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gvzyndlli.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqawwdyju.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gwqbftyww.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gmjipydll.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gofecfbsv.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gdfpysatj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gyttagiin.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gqmkxijfv.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gezcprhwa.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/goucivolr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbctvzuit.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gsjvcknqm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gurgelcve.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gdvgeufph.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/grpasvrtj.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gqarmburk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gqewbrfue.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gefwnvmxu.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/ggiralpnb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/ghrmercqf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/ghtoxhoar.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gecucvtfc.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gkeybvcho.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gzotrhybo.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/ghbbcsmmw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gnzbamjic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsfbsuybj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gcpgituxp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gxsrlvkqp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gscuetknx.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gqepyaibe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/girzmnqea.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gobkwssgn.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gbyuvfrbb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gjbmmtbzq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gacsqbabj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gjkzwmwen.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gbxtzxdtx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gtdyyplch.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gyikhlrue.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gottgknfm.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gifguzzhu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gqvppfnrm.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghmgxnirm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gsfkexfvm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gpykthrha.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gxcsbfrcc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gcwbdxzzj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gfvpqpdzt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gewbnazrg.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gsjvtpnnx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gqxxsdrmt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gqnsbihct.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gisxpageb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/glvkmuzbb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gjfbpsalh.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gfhiklcjj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gjlfkfmhh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/guxirlgpr.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gzvickmhx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gewdnrxer.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gghobwzcz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gxyhhjqse.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gurpbzmpb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gqzzonpcw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gmbnqjpzj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/griwcfcxz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gakoouipa.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gspgyxgnu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gpessfcht.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gpopfqeyl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gigjdjifk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gnpixcvcb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/ggpntngrl.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/giidnrvkw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/ghwydmzon.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbyejmgix.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqmpgmclp.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gzilrlhvv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzqokrbiq.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gmotopxrz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gommgedva.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gidoqenus.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gobbiuqfs.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gzqjrdczo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gddjveyfb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gzabcbwtl.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gfxxpvnho.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/geganvprt.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gkeqhmgzo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gjgoclapa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gjeqvujms.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gtyydvzlz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gxkizgacq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gbkhtcjse.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gsrlmirea.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gziwqhino.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gspwgalzk.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gaskcfiwu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gijqorxyp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gybffindv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gjiuublxv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/grwjqztql.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gvunygtep.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/geaapisfr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/ggapsxrsc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gdduvclxc.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gflmmxgmr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gidcklrno.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gnvxdrina.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gzprjxdah.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gauisxitf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/grmrkyhet.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gmslpmkwz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gkgvpgust.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gdfbamdzt.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gxvixqmfy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/geqhoigvb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gnllzbnzv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/glxajabbg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/glviugtih.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gofzjizte.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gxaqxhczt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gsqsmnnxa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gfohkkivy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gkslckicn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gycpnlsng.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gmdvfvcnb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gsizdkdbv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/grduicgdr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gilfeedxb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/guukjzspv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gzdbhffwh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gbpkpuhal.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gwdacwshq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gsapiiklo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gbucxqnjg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gadhvvggv.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gsxfywrmw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gmjeoyaly.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gyhedwlfk.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gxhqmufle.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gdhmqhcja.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggxhupdde.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gjwtintyc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/ghrsduzth.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gkekfbpld.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gonvbnfmp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/giwylcxxi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gpkzqwxvv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gxqjatmmk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gxowqfllq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grxyhyvhg.sHtML


<!-- 参考信息 -->