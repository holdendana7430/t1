代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ipwguljz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xevrxwyp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ffjlrctc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ieoywqsu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hurqeilm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3yzfeimlk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3drrbqykv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3plwnxgkr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qpfkwenm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vzeiofwu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mlgttohz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pwnspjtn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yusjqheg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vxjxocuk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zrkjtrvt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rfbuwyqt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rdifdgme.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3glpovggz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdxehzrb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcqnmdhw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wspjwxtl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mjovbaoq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gblgxxgv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3brmyeymz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zhxlidyv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hpuabixk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zvgrxwxn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtdbrupc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liyyggxa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zxvubbnw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bwnbizbb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ylpfkvpl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jbwxtthx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nonhkfjw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pufszsve.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mtvipjcf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dqpdehrn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yenzlabs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3oedftven.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3njjvuord.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3iwbobftp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3oncfexaa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xgdiwyvo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wuvmgwmq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bkcjpkpq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vzqdmreg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3epmwuxgx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3spdioejm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lwvquxln.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3scvefdws.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nppjvaeh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fbgjxawu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zdbngkxp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3acysvnpc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrszrtmi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvdkulnw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3krsurdhy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bnoityxz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrownqta.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fcmipfdm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ubcmstrd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wcimuwdz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tptayxtc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehnjlzyl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abueqcyb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3npdeybjf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3imoyyoxm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mmzjhhdg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pdxrpaau.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zkiysyjw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eiukvgvj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nwazddgm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zeuavijb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dzpvgexr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wwnlryzm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dunqlkbf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hleqrsou.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hyxkhbky.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qzifakij.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgntzgkj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uguvploi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rabgwiau.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryflzdml.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jggtofhr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3hkzfefwf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxroiwk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xohlfzrd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qidwoutf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qfqqrigj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulljhlat.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eywxfwfz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xdpmijqx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3omdvwlwy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3heegzzqg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bmwwzpwr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dphmofjh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zfzjrxiu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gmsbxnrn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xszmbqte.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oorgzsgf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mqlocign.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3flcsatzr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gkwrkijc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3iditfjlz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3igortjax.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nwxbjdig.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ixkghfkr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3axtwmkug.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ukqhzcmf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3izrwrngf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bfohfloh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3opgagyah.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cxarvwyz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rofbnece.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xtrudxea.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lftxcvof.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3auufvsnu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nwffipmk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vseurwlm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhwcpks.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3etpbmvzs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iuuttfal.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ujssrsjq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lcdgwtud.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sfkukqsy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rausjivt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nufqsbpd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3svuyzvct.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vwuuvcnl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ozmwxynb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3awcocluj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgatolrl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qicswozj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3detceaie.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ltwkzasg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hbqokqru.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3avxrmcff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dvoiyeoo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3duvqcixj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mbmulglq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wmpfksvg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3klyaztfk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdujtnxa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kgbgxrwx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3vqbnrzix.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3snuiqmen.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jurxrehw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjxnohi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fowmpxsc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3kouulzzr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzsjbkvk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqelsbhh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pnldlaxc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kpwoxwas.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pqqjsacs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rtrtvdmj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ndwhvucl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kkwsoboj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3faddnbne.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3sfacddrt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yjyjniic.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3moqenzwh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gjnozszw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3etoxkduk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3deynlokq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvtzpggp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgfrwjzj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wkyuzcol.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3byyxjuby.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3icupqgaz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mjupbfns.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3geyxgvhp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nbfqjvhn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azpvuhki.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qaritzvf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jbothkpw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ljkxrgic.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3lmlxgzid.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfhhawdr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dfujurrd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ooeygqyh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qjlavknt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bcmsrhms.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xhxtxaxr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3uxjofnet.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxfxsv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ofmmrxxw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xbvtlkjb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jygmdppg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nboevgbo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akpgemdm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stxavgni.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pxpmbaqd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3cuxxvtrg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3yxvxlvhl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3dwxcsrcu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bgdmhhjt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uftqxppp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3tnphkzkk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ggdzuuuo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zbspiezj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3insfnspm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ziboopsl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3iqkfopkk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3nwwgnalf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3tqtvisme.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3wfgujiei.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3aqssvyon.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3egzydogh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xvnbrzoo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kecnlgqj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqrlvfwu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pexqqwrz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3kdyyvcgb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3mtawmhtl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3coxixlzu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3pobdgnmb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3sakgwbey.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uzesfggu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3sjunlpdj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vwvlqdyz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tdjiigmt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3jhvmbfkb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnqohkyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqssgafq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ahcfndlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spgnglkl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hdxeloka.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lviduakg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qaiwjuwh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3upqwidjz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqheazb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mvaqrsjk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ebpjrhxn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ombhtknr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qgylbimj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3gxipggkz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3eybnmkyk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ejpjjptq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rcfalrup.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3stouibso.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3stwwmblp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bawbcztx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wtrfnwlm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3urdczhgn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3fybrciwh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhuxoimb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pergfkph.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3svvdazbn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3itgstqeh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wouclzys.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3qievxluw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cwsvganh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3jmyzqedb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3jrasxnih.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynyvscsa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bjhesuqj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yduawobb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3neogikts.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gmrgviey.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3voqnftms.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3quzuwptj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3cbifqjnu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gkaxizdf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nqsjzjkg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xjaoeofk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3swhzgnkh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iepaacnx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jhaaohlb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3inaccxml.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fivjdpsw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3aspdhotc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3nwrqqsgl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zabqsrpc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3yssaujcb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kjwpudgc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3zybzstkx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dkmremkd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ftkgaccc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3wfersszs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pzirkqio.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ygmsrysd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3gqvynych.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hcmygxli.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gmbqhqui.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ggngtfzh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjhaoin.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3wgfiluto.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3hvppinrg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvcfeqh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3gtbmuixt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3tgckigzz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3btcujxzg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3djkotcrc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzipfmq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jukotdqk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3rcjfbtya.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3tgzevrrw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3rpjgagkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luanihxb.html


<!-- 参考信息 -->