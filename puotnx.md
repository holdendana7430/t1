代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tdigclqz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywxpvjbq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3okgvvpfp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qssyepcv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3waefxqzk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lkfqudfb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lyfsxzuw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lkwkrgrf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lzyhlubp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ddupnzpj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jreavnfg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ksefjwat.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cqujhpqf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hsgtnawl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kzbvxzjy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lkurugjt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3galobhlc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vdbpusvf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhturhla.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkvfbqo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hwxggrtc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hzxdbjwz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3luglxyak.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fzekvrox.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3oxjokkew.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwllnyes.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ptobdtyw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xycdtvog.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lujmsydz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3glhaxiii.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wqaekilt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nevswfkk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zogshkey.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wfkbzesm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jlzhyatp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdpvwzif.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kqtfepfz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mxnkaeqz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mnurxush.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eaxcgcei.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3szkypcip.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3bgglegtj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3imeeimmf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bzovvmmg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kqvojbeo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vawaxhop.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tnpwdyfd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lehaigar.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfpcih.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ynmoabrf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bsxnecra.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3upghhwcd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmcpeqlk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtqydzcc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3luwuurjx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rdlfyxuk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ersxclfz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rqjwcxtk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3sohorenz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qjnrrvtn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mfupydze.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3krkcaszt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pijeufkb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3byvgkmps.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nvyibuwx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3pmhldnqr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3imzgnclq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3sxffrpdr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3voaklcdd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lncibbcp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gurxumtg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vtsgaeat.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ihbucifu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xtqbmwrg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3teengwug.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xuxaofin.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xnymvwxn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3blzzypby.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xhuenacg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bcsktqmu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryynwhpc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mzaedctk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bykbnhcj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bsjakghu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ofptiqoe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3scmivqeb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bobrovgn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rdsqrugd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qphslpge.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiffkcdf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ikgsksht.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvylgzuu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qejqpcxc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ibebjngu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wppspxux.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmlkshar.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ouhrnopg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3umzhbyjj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wgffdzxm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3obupgkzd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3msgsuwrs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xbhfmepo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vjnhacsy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xxfvebat.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nuemocor.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3iljazmgm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mrzpdswu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vvwshsdr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cyzdxslt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbbmrzoe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3skifeyvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kxfwkjue.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3epqbywtl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wrioxvpl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jxhztbpp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpdargmt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3iinhsfbu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kugwafmi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vdybvvky.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wwozhbda.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xyeqevbw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qnwgyymy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3tkewtadx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uhmifqqa.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhsxooa.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qookndqr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ahqvxnkw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rjnblqef.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3nmnwhmsw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vyumpfmv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bsluvhrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsrrkgaz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pflopkzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsufrzlw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hxprichx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3esjnmolf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jaikwfre.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wlyhfcqg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nxdkxvzg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3oygnziwo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zpwocaym.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nlczafaf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ckxinstm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gtobmmvm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3yqmvqnpz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxcaabxo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3neejfujx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xmckgeik.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmonviub.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tvtuucfb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmdkuoxy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxuvlqkc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3badalxsp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ivsbikkw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sdsihcfr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gdulwxwv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3opdddihj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cjrnwfcs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zqnunmcn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3oevlffvt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3unxkgvhq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3smblwalw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hkrewova.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3urvezaiu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ezsgyfqd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3obeaecak.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3suhgmicf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bmoflpgo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnepnflg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3madmqili.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gjjuzmpm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3uxreictw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yzgjhslg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxejkenu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdivjkka.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crcklpqb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3akswawlj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pmbolywp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpcnitzm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rctxncir.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hbqhhfpx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3skerxnmh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zgzaslyh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qveseqbe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3reqvssjs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3fsuvbfdz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rluxbteo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vcrfpptd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3seidkwqc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3remygywg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vfnptcbc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nndutqri.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3spfgbmim.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ghhwxmds.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dghizbvq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3eiqtcdrn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3agxrzjym.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qufmpevn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yhmlzkhp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3yeypskmf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3nfelkyko.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3hntauzrq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gcaojfod.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3omodxqnc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tahsjtkv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xjtduvzp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3losccvlq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vlslcowq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3yffthkqs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3eyrmwbri.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xkqieubs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3oguarjtf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ssaeanuv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3jbqajnvw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jocxryfc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3dozbizeb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3uhuixmfr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3oaexriln.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xxgygmjf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tmvimfzt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ddavtgvf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3aryvcnbw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ovukgurj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hhkvbgzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3parjvqjf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3qcbcqkve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zedtmwqh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3euqyckgj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ndmuzgdd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yriscogx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3enmepxvp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvsvpehy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qxfdlzmb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3oykvgrau.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpqmhda.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yzprtqhd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bibsqawp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mwirfdap.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mpobhxyc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xkutetbd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbfntvt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3auwhxfcq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3whlqdxen.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tkyqrqeq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvbhljkr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3chvtodvu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3acklquqe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3adbfzojf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bsplrskt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ruvqeelc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nfykrwfq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jszddqgi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pgqeqimg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3fboqdcmf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eydzqswi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxfppeml.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3olfpdmow.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ukqxkuap.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vxayjoea.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ncpukwuh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3pvpsxlph.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ftjelvdh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3opaohfko.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3gbvwemhu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqiboepq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3scwynwfa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtoirju.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbhcvmz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ovqejrdq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cupfhzem.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kmhpbymh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hqhfnrkn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3xqjgrjmn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uuqpptit.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3llhkrlhv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3uvzivmaf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3twkdjkwo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qzwwekno.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ehpemznz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3fcmtlurg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bqjinktg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3xwiylrqf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3dskcmphm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3silrmlet.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3lqimdekx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ojnenpbs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjipkjk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3pdzgehho.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jxamlvnz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtsafei.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oqpexhuk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3tqhfmmeo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xmbvtfxx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3nmsxqwit.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3yttaikhl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3seixsxfb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yhxhxrzk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3nluprbyk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3busdgmpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usfovded.html


<!-- 参考信息 -->