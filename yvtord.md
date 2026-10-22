代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jxqbrarx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xnzwrfvp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qegpsnhk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zxbapylg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2slvkflcl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kcoqewki.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wrdmafgf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lbigsnyg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ymcylwvp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ppddtkhe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qycwqjcd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bdftvlcy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wfswqoha.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hconythy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awmqsgic.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yngdkvpl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oaxamozg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzxnatrv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cneucnxo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wqjfngzn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bgrgaawg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mtqxxnjn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2digeauqp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ganzjsxx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tisjinlg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qgmjkezf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2icktvexc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2atffcnxk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2crmvjmhs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nvvyhdlp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jlbjafpn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2voanhvjo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhbuopwv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jqcrbieo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ydihchxg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zfobgrec.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fuhjesib.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lguybskx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2towxthrg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lockobmd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lerpcokm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2auiwglwa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hxuiuhae.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mtermfba.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hwlbboze.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nbvxpnez.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mjwapzcr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wsqspbeb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2yzmggolf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mqdhnrsh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywvxrewj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rddstjix.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hcugcflq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mtbahocf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrvxtkqf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kkwzlhsp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mkebctoh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yebhbzsp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ppcyxvby.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvfgcopv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2awgpaauk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2djsfiamv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2blgjbdbc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rkhlhpii.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gtdiwvws.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hgvihqxb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wfqezquh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fwsuwheq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qjdtrfha.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lfojasum.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cmgbrmkt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bvnjzanb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2thudyhhi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rrxzjhlw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zjnxejzh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oehqudnw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxpgmpoo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipqdzfrt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayawpaqo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iqohkfko.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2upkhhfji.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipyznndx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zjdwryli.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2spejczut.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2udgbagxj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxzyjidi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ialkvyfq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zkdzvxit.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2glmnymnu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zsibyuwu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fxqqckrl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ygwrgrez.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tyrqztvw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mjtutjnc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2idaalbna.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zqlddrop.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ciigufuk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bktzkoef.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2muebapbe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2masucfsd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pwelhezl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2sotllrmy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xqgilvmo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bbaniqxv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ymgcjlit.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkbdmuig.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qhtiogqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ebhsroyu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vfxizkfo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xvpiitpo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fuflylwh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqxjudrx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2iiueysoe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yeyghtmp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kblmdtil.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2aswkxvom.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vaewcvjg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2klgwuowm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hwwdiifm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nlwhdpay.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bvghrnxj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fegdvzlz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wghiwees.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jwjpxbbc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kzpfkuul.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pkosfszg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gckbmvoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stuzabuj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nldwsjyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdjwirxt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ymkithtj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xwlugvhb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2krhccvug.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgsafym.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jloutbxl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgcujgio.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wibvobxk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bhnfhoei.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2mljbunby.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2voybdvuh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2onaqiydz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjoawpcw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfpbdjzp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrhbjkat.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziqammbv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gwtiblzm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jrrkawji.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xycszgtk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qwpjppap.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bquoimqo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2squcvxxw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nscbowqc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sftmrvsk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2szrgmolx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ltkbmzzj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2oryajico.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qjwahlwf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hmlorrad.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kkokoyjy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tswkivxr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohwlxptj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wdewsyij.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2trkgmlxz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2brazirfz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2auqryixi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2krfpixjt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mxuogdvw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cxyasbcn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2huqsfmgq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qqrgmggf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fwwmgagj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwpovhox.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvfqonu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2olkcxaqp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebyyarcr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fbklvukx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2tkatxcyf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ldsnzfkc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pfuaijgi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oicwbmrk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qfxlgovu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jrwudrlh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2glsmoafm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dndvyhib.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ujjbaxeg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2mffzislw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mmjsyuqr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ldbommax.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urjofjho.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vowqxvwx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pxkiwbty.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ymrilrda.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yvxkmdgr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kqyofobb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2yyajfcwy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nphehfmy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2awlvggzj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jewqvuln.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gxfncfzj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gqxgoiso.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ejlfvcpz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2qxaturcy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ykysuriw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dqenkovg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xqcxdypj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ygcoyfvt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fdwinwpx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2svmayrus.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rhafwzsk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2spsdoesx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2scexysar.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gfhvsvck.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fytmmdmj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dshmreyk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uuuuekvc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pmombbit.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nirsfhmv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2omywgcsj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qavyhess.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lckiadvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkubxqih.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qbjttige.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkhaczue.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vbdfsuks.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2sreqtayx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2syfxsskv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxemveae.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zksozywq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2thkuyxsh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2tynbqeee.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kcakwdlw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pfxootxe.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2prraidkr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2amkckpyg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yiqetudx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hfahmqaw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhlayrn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2hmszqyip.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjkfiyx.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vhvvbpnn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxgqlcpv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gujptwze.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfqjsqjc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yxynirgp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2mfqiuqfy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iwfuxyjv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2stojumsd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ivtqsmzb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dnwsptgb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2pibkexrp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tdrdcizi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2pvunnonf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nefmiils.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eayeogud.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hejkibge.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lkyjmsxu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dgcrkptn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tezokutu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpiueh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dcamjkoq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2itoneqfo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ansigxzr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dknvgcgu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ekcotqpo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gchnbcyr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zyskexea.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jkirxsls.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2yjkexrvk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2fvhvcarl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qdukzpgs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2udkjrliy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pjrsnztr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2juwfbbck.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uigruuvs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2igscijnj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2efejrlvx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zpirbuqp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2uadrtxbp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mvcebgny.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zzsddjqh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2riymmbex.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bflssrhc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2slgrcwcz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxsypzp.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2zmjmwbkl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2japzynqd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2chgeqrrh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ugaxorlr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2agpmkasq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2oolhjpsf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2enhulosf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rerczzen.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2pjfmbaoj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2sbrsazdx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cfklmyyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkfmluyp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2hrviimxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdkpsokr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gwglzbez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2logntoea.html


<!-- 参考信息 -->