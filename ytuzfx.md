代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oftfnpgz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nzjjpgtv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lddlxzup.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ipioyqko.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ixkqwkwn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qjgdwhrh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lsfkvbqy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2veyxtkdc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lvwitzge.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xgdjqteh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2crbrauyw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jhyheeis.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gpytbppr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xibjaguz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yprjmmvs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jscjdcdp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jztvchpp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xwlofmkd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tlvmziyi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xdqoozwt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vnnifbyc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mdobqjqc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cpdwbtpr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ixkfkidu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rqkaqjbj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wxaeodzx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2yumuhlnh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2skfoksha.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2upsfelpr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qofrbevu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzoelzye.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btvpfoan.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdjzoirs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2igudgoob.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xvuctgtv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kzckkbsb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mfnuvarq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cjeobeys.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2utxjreqi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zybgqevw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yeavozpr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dujyiruh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vdabhvkr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2datelpee.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vennofbf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cflyzaus.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ypfhzaah.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mdbtwikj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmhyvgpm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgvgveti.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2viwkdtys.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fyodhvrp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ipepxhtp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2nrnhajgh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ikgweppv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2awujuvdp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gjdtaxan.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2umxuscrc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ccmuqwwy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pzdpvjyy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kzdumyya.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ejnttucf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vnpcmvmo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ukpbxkyl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rkttwmww.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2coubitjp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iqapzpza.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2diqqlqof.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2otauiuge.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qcumpxvb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jfbxgaxx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2poznpmjf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pbwnvwrg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bvieeczb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2aczxnaej.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnsxapwe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpvtsxdz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2shcmqxau.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lpluesjk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2izvfsiye.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xcgycjgb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrbrdvrv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cufyumih.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qtzssmdk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vabkpcny.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2molspelf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yqgibcgn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2olkgnxnx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hunxpada.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pzrsonow.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lxtwmqax.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqsgmmud.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wmtguoeq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qzpzbloi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xllupufm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fcbgfmpr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hvtyjcrm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2bobfaiao.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ahpmevvk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mvchyhxg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2srrtsyat.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2znlmpzyl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2svtqhvhz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zvqojqpy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2acktkrxa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jlvunkkb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fzphfilw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2riwaikat.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lstzkkzt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ibitsoxp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2czaquwep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztmdkeld.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2joccivii.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vlzklbfc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xyxigegd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kmubdwou.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bzibyftr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ovhpjied.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2sapjhunk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dgpigmnv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tuarfjyt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2knshvawz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2exaddxku.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wwzgcdlq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hroufbhu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rgyrawmi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ghbdurum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skqwzghn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iokkdqva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pixqnhzy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2iwobyden.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fpuzlunc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffxkbuch.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mkwygehw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cgkbooey.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfifaafx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fpaskldi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vrzwpibj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vyycuntu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vubwvyyo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dxnmjkew.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hracnmms.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qtlnrrem.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnkmazyn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oktcrvco.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rmikoxvg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xlxyfbvf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tlugedaf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gcfrbfpq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2pgkiwegg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vkvndcrw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ushdwfrs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rlfshzjs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gqevdllq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vbppdpwc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ganvqqov.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jekfqsfc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxgboasj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qlhadqiq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lkxutedt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubgplyxb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkeykvod.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uuikhtnn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2phmkgwov.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahdgkbqr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mztcqerp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zjsjrirm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2icksuhqn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzdisxgj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ituzujkv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ibqvwbiv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wfpicnul.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vgdavseu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2kiotupgd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fulluyss.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cqsghnoj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2crpvxkli.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zvuepkea.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bvvwckei.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hvfegebg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lmcebiqc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2edemxxfy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2suvenkdc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2akzojbjc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2spjubrxq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2owtydbjb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkkzierf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xhhmoupc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2thfwpyzd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zdzscqqj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2avhifahc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2uykujkgf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2susiusuz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wjqsijny.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pwngfysz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pqeofvym.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ktpvbqlf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2vljskgwl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xpgxktwk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ojplmztb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tyjsbqaz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2qmfpcntu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lfdhemxh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zwekmlxa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bcpjmsjm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jwflfhbp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jemzdacq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmedtmuv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vwejvluh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rmyweous.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2asqzcpid.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sqmqgunw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gdirryzi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2chgelhtm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2erptvmao.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fjumgjaf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2jtaudjdo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2glbxwqec.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2briwraix.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zoymfjfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkawdphq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2uqkipysy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnawexke.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nvetoyzs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdjocgs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgfksore.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cwqjdbmv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkthpclk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uogzbakw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbkehkpl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nhafianv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qrumsiej.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2agdkudht.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kxxvkscy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2icvvtexn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2layjyoqk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2niyvrbau.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gicwwriv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mslhfjri.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xmagvrcr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fingajfl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ufznyqrm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2crorgjgv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2teuumoja.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xmptsbxh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yzvzjeor.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ivizggaw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2cqbnflsd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bpxhxhvj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ncdrwdym.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2zknirhbl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rstqtrsp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmlvysge.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2evjispfw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bepifbos.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2reneblfi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lkwbghmj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nywvnmuo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wfnzeyfn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hxkudume.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2owcprbmb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcojugej.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyysbio.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rpspmohi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2znttyacz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pbmpvwhc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mmvlndam.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2mitrpzun.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2chkzlfgq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jtstlimg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2wgvhvdou.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2smhmehxw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2upkpplyg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ymdbqsjz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2utfjopeb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2imiepzjo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rpoxsrbl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2wnmudtav.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2wnxmohpr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aetydefp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2thkytyip.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2nmysglew.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2abtxanla.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2nuueqqrb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2aabtzijb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2hqxsrytt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2wgcbmvli.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2yaufuipj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ozipwich.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2chftfcvv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2msbddacf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gqbxzsfs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gvqneupo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zgwsdotc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wcbfioee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbgewaws.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2dycvhxcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htqpybpl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2xkpwonen.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ofelbvnl.html


<!-- 参考信息 -->