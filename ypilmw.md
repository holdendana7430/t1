代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ptmfvjab.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hdmkkrhc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2irfszwjq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kemqtlwv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ynlnjsrq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yqleyqxt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gtwhswzr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tqxiancc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eenspcsx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qjlaxumz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zatotfxt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kamvlozl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qbtgdsax.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aooutrmt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dobxeyln.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hdtcslgs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zrqusyzb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hczariov.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwskeylf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdpaahay.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdtmbned.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dclgcgdd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zckwzivh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pyofbryv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wwaeuluc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wgknttdj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fmdrvihp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpcwfmlw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bihfefau.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvehvcij.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jrlltxqy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gsvrxqeb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2utpzrrtp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jhnijqlb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gdzdfbbm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2muyctyjq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lnajtgmf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eazwhjes.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gtcidopm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ymcjglix.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2iycpemxe.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kdqupbad.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mkwxvttg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lznvunjj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijwkdkot.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bovkrtwj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvfyclwq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vgzsorxb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ltubsazc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvqeqjsf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tgzaiath.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ibyybqvz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qoptrcli.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wcpfmzuo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bdqncdax.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdrcgqzc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvipajbw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xrngohly.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2aglkgdup.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2cetvecbf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2smxkepsv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uttrfpzd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tmvmhkvs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mzstzarg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dwhcdltg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2julegmij.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2botzioln.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jmndkrfz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zskbontf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ybwmoknc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zvvpelbb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuarnvyk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ejjrkhra.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugforawn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tyrkvxrv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tqtuzuem.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gzigseoi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmqksbt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wcwqcqoj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ugccsiyb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oewjnjhe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yxcvndqy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2upwepdbe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssmmasci.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2odynltaz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sfdrrumd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2asglpfca.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ehrmxvhw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mbozajfg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2flwcmipq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pqrgiygp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bjdlmxqs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ewatlzgc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2rorobdqv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qruferrm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hogjdrln.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ufeizbvg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pdeonnvy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2syoexrwe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dyetogoo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mtrssvgl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ukogwmbt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rjuuvpsq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nplvffzd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2omcxzfhw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gmbesayt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ywrsfwbj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ipommkjx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wzhfheqn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ktdobbll.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2hmlkwtty.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xtokampc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2eipkopfu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ygaozsey.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qsynkyeb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xzdjfxde.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2higqrmtm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfauxwrj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ekzntipm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2axdbwzrq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sxzcftjv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jowikufs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2igasmjvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbucwisr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tzdgpiev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpaiautp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nckfpcfx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qywrwwhx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cwhiwzaz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kidcbadi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zpcwrmqu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2orckrdbv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2yryrxysd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ouslwvoq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bgvcewad.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bvxofzgg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2myuntcmp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2euspbvwo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxbvmly.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxqrylkj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wcdcohsy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vtmtulmo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxgfxmut.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2giwooaga.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nxjgjuhg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2eypbjdqx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mezgwsla.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mlheorqh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rgslovae.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ddqwdgwm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2opbtkpef.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kjdhyyqm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2axqcrubj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ysniqgci.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ekjbxdcc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2osgmjoih.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cppjsdni.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zbqizyec.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dzfbrcvv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wkpbnxfb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynanamuu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkryuwom.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2edauqveo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2iakfqsgq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2oagjaxmf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmqdtjyp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qkbdzypi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jefpwqri.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hbijmxfu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2voxnrwkh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2grjfecaa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ckdfxbjm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qkxaudyi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vowwwcpc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ucuptnoy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oxlcyzvt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2yinhdyhy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2pbxsiurk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2eehhdnfm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rgzyronu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rbkcbpex.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2etrhwiua.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hnnkiqhn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ebilgzfh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kkryngph.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ambvfffr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vfihzofa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wmmihljl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dwfbeifa.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kzoaovzq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mlackxyt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yayjzhxt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2srqtgpmh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2iaqoaykm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2nagjlrkf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hooloipi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bffyctlv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lywmuwjx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2siimouql.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2cruaoeuq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tynxxbaz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2izntrowq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ffzghdzo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jznkvnqn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2wkvkpgdo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2sqfjdpiw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2kmlddeil.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2sjficpwv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xeacimui.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2cemgwlib.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zpacgbam.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lgckklwr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2gymdeoed.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nnosjsga.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2trhtdbak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbjwlwtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsstheuv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2grdbctux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqfbsclj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qrqneusz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbqzkzk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bseometx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nmrdzpwt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2eqlbfsgi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lhtbhajf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsvwthgq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bmpvrmle.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xfufvtit.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zapoljra.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfduupyo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ccbbzbpg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2easdwcjx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tlsfybvk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rkvoqgal.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2slnzlkfg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mcqcbgon.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tbshtkeq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dfxxrlpi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ylzqukhn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ydjokyql.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ofkvnhcu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2sxwsqzkb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jwxghuxk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wezjkpph.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2uutfbdce.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2arlwsitk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ndocbnvd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvivgms.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mfwyevbt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nuxazxln.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lkgnqzha.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2njhewzkh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vnjgiiku.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ttdpsjbk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pqwnvuzm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sfalzkyt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xeihmxat.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sklxcnii.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2msbkfclr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2apwiwtza.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2snyfhswf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tdvqmozq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2awkyszvw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2unmvmoqg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2dvoyjygn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2efucaecy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2hcfrtnfk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wdpcrcmd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qvwcqefk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iyiyuvsf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2yjqlloqx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2zqtyhfgl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cfwqumnb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2bedkwjxc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2suavsdpu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jndaarmk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2uewqzncs.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2tfizpxka.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2awvpeedi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vfqlrkdt.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbbbyyf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2dqclmqwd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gahllvgx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2qfqqvbpr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ygofwtkn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iqfdoinm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2halzbxxi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2puupgice.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2wceutzqs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2emkflnhl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jooucqhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rypihmwg.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gjujtdww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwhmpbju.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2duvybpal.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2gmiurzup.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2dynoyacd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ygdbcaft.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nuhxwhcu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2mmnvvgqc.html


<!-- 参考信息 -->