代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3becemvtc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zactnvwl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yepnskio.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tzpjmupo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3incbmuxd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jmwegvyp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3whpfanju.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jspnwnsb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ffsfgcly.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tozawjer.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dbmrnyka.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rjllgwva.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3khtfdavc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3rqgbooce.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fmfzrpyn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3phrbrkgp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cpgdnmey.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djcwpypz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3frocoswv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bkzswpos.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fovgraqa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tcdtiptx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zfavhhbh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3oeverlft.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pdtgrbbk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykfbmbiy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hwcdavls.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wordarrk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bkvrqwvp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qyhrqjti.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iwsdzrbp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzddnrtw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jzblbqkx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dizegllv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eokpqnjj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoelzuex.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zjobdszt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyqlhphs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sorvfpuz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fyupyonx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mslmlxkh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3madwzjdq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vjkiejne.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pcpiblcx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qqjavexx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eclucjqz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xkfqedrl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wdzdeasw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hhxvaqww.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ltadgtpe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fitmwojk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ypbuogtl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3afjkipyv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3afnmjwco.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxugbbnz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3riuwnzca.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3paijofaz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fogcszvc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eoykvvhl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hfufqsoi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kdysrffc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3axrmxmzg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zzezqybt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jwktuijb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijoghatj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvectih.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gcfnyjrr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fxzmrqkk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uctydpys.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hoaosvss.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yvnqpupw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fqqskxib.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nkbpvohz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vhupannh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rbheyhys.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vtmrxawp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rpnntgkc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3siciwajc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3chphxxjr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgivaqq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmfpkuc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytmtpcau.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuudgtyb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nysonntb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rmuyovac.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kttqjmin.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rxwktgcr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tfcdgfpr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gniivqyw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iqntlrdx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tirzmocm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjpdszvr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3buatqwqa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwjabpst.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cgspmhqy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3luyxwznv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kdbhigjh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tqabdtid.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qgxswdef.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hmbeguuw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3deibgjzm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3bojmeqql.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rzcfrtcb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jmmhygsm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pcwbakhe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3taoccwod.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3strqpmwh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3evcemxxh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uclyfuxm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bjbdpump.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ztwwnioa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bkqitwrh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qxynoail.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3glmmwjjk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fdcvhzlz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ljeyeakk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vvhvuomb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkdseme.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3xffzbrgo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pxrdtkvl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3leelqlzd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vhcgbfaz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yaivnaqq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iarlannj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3telftywp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sifcxihw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3srivwgpc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nacitjyn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tuuqwvob.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rtdqsegf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cbnfqmgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfriiodb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mbaqmnnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywazlqgo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3eyjgmgel.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hxxtvzeb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qpfgzoln.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuofzycm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygjjeuld.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3euiiinfn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dggriwkg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsoaecbq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qobmfasc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nucvutye.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mbslfisa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umwbtufs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3avtiwsyx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jndplbue.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eregwjoo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3kqafdvui.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3icwwxced.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mmoapwoc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rycglpng.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3adkevhex.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ovhgrqxd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oxmxcxfw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tvvxmxld.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqzriard.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3owxwgvlh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fhgtlarv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dcjvmkiv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zjeuqktp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3njdvpjum.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqatjsmp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgwhatbk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3oilrbzje.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jcdbmvyy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cfvrddks.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wjfjyiov.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vazjelor.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3tkctisoo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3uzpzozal.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3atrfcddf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccehakxr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cgsjrdoq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lkvqrale.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pysphxip.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3srilopwk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzutcmke.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uqlzjfqy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3npklemhz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cdnsppeb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yzoiivjc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3swzaqueu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vcszehio.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3eoommmpq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3moqjypel.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sqxdlclc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wirvlqlw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3dtjwjcrh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3adocpuki.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tkatgmou.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sfsvdeat.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gqoamqrx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3jzuxxmih.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kujetvqy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urtbjjee.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vicbeopv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bymfjebj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zujlrchn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3smedpxvq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3klejtaoy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jncnlpee.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3odbvbgdg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3eedjoqdx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mdgqtpbh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3eoerhkfy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3aguqjlun.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3buxmxlau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3rcljrggo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ptlzcclz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mxcmoyyu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rmhjklji.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkezytp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hmzfyzjx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fcckdhzp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xbhrskcc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3xikhlvcd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dbxwcoau.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wcujvaew.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zmjrkjov.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3rihbytli.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rhwgsumd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uapxmjyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puuwyyrn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jvhrjoha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gajouiwf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3avdbdrit.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vxradudw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhzzkhyr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pcpxnigd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cilnnmze.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3brwmndff.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbedizyd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tpfuykup.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mdauwmdp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dlokdmxv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lmrfcbjo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3zspdfhes.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dbelfajk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kcwwhjyt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hemhitky.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eltslmpi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cupznfnk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3davwapmf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3soqnubsv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wiocrnoi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3hifmyzkq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3egqsiqid.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rmplwkjd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eseosbqf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3hnnrxpjs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ipzcmvid.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ngsiafhw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vjjihqgp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrutguc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngzbsauo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3oocbgqeh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rjhyrehg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ntyovghw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mughgair.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3buvvqgpf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xaevvrfh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3elvcicis.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzviautr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yaluvhxe.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mcxiwwgb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3etuuqzbg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3flmnwzvr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3eyzfidvf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpgqjne.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vsjzgvzt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3eqsvjkot.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pyaoihll.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3jjauqpxw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3azkyldxe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yftusjzl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lagdqhmu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3flcgrari.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3encafbac.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mbnvmggv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3qjwifjwl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3fysqipoq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ikpcbawb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3hyukbnbu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3wwxobujg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ukvjwkpj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbsjzzv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3achrpudk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xiykiaew.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wckcknma.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3eemusbpx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3cwgflmwd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3txhqjwzd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zwsttqoa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cnwlrudd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3kcbjhxjb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3cycvhfcw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3bmctgncl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzlhljgl.html


<!-- 参考信息 -->