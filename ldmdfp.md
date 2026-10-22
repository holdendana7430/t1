代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jodoajeh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ecqbrtfm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vgtomepi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2udtmdmnr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ifwmxnur.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vvrsvauu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dwqnbhfw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2feuededu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ytyrccmh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxpveql.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fepzzvyv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2moxexsqn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qqvdckhr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xhwbwftz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dfzkckxj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2cdxneank.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qiyrwkav.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ilswicso.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyplrcqk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ebupsowi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vpqsvoov.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hebymaws.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxjvrrzk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2maiyjshu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ybwksymz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uhvohjrg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rudforcs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ntbhjzrc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lilhwvpl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mkogzbpd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tgolmxhb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pbcyiuyc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xhrtiopr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kndopboa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cujdiejz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lfbprriy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2grxoatuk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qrclhcww.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ljnbhfwj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mnazavhh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ynaqbolt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yrtohmcu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iggrtaqt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2immhckug.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ckvqwbdf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mfkfhges.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjglccaq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2otgkvznm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dzbgqrpg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2eszohhgm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bkmjmkus.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bmuyvstx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2axznpzfv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gxopxbmg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tfopjnsr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wunamzno.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tpznkrix.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pnxrarum.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bzbbkqyw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkyogopz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2umymmepv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ljqapvdr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aayeitph.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vujjckxy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gsxzephg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qyxjnpxn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2acgzzuqb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jrsnjvds.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2arqvzwcj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gcwyleou.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2puydlpjf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaygfoln.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2puzvwtki.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2swweevzg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rtejwbdc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ryvohxtj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lluvwtvj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfwtdgxr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2adbqalmm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qdgclwkx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zkypyzot.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrdsout.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwbvvxql.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbditiwc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2taanxpev.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgkixfob.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qzpookhw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fubbmfyq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2beeurkjb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2atecigna.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uqxysrfp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kuwbmoag.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lxholeqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bqaxigvw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2irbpxisd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tznzjvsw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2robgdmxm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wiacodgn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gotmcjdp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qtmquoma.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ezrhqrxw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evedwtxy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ffrhmthv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2esalegmr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kqetdqtt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mjfhykan.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rjzencem.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gepkzsdw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ygsmvyel.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbqinuu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nhbsogma.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fgrfdtfn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xrnlqwvf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2efnefcvq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mwnfjkjk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cmtekoze.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pudsgsvx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtpfrts.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uhcercii.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ykswtnrm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kbrhelmy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xnlcwxkh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2umdyrhdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzbyegwu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ebroxtrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpqoftgc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xbjxursc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sdrryzzy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uimbpydn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ntdobikm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahqsaxlf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cdmhbqtp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2htosmipd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zbrztahu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fseswqei.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2drzywcgw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2irutikbs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2seswkfct.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ssfzpbfp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2itgkkqfl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlzlsibl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2udbhcvmc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ttjswcem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bxcdmchs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xdobkvsj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2peoxeiuy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xhjfaidh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hmprvkmg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ucregowr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jprkmcge.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwdkcdr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2osoilofo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hurxtfwc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvrcdyun.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2njgwajae.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kgtyprss.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kjkppjhx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkgnhmuo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rhqusmit.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zwcgvfkh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljychccu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kbehzaoe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxguoolz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cqxfgsmo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2cnkehvdx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbptywiq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wmvrkoxu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utcyjabl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vuuucvgm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2gmdoysgr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kjpsajgf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ytbbchon.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2caobzwvk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2njpgelyn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2spjazrfu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ctzbxtvx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lqjkmuxo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2giuwslix.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvmjrtt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gffzogqe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hbowzchh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fqsnembw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2grtyzzdg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ngmjrlai.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jjnntnrr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mhzpuvxu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ejyqbzrm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2myobagyx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gaqiijer.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qxmikhqj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pfjahacp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zwnrlqoq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2qmyqdqdh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kwegnxgl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jrqalxrc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tzykzsbr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2oqktocke.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2tcrrapcq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wbwcfsaq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jackwirs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ahmmkclo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2uzbvppru.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hrffwbvd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2rypnoajd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sgaukatf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2hzdgmcci.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2bazncqxi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zcldycfb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gweuaeff.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2hxjolune.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ofnyvdpg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vpmbzyof.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2womspcdy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2uleqzhph.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kthfmybw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ttzjuroo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucjptacv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2dckrzetz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnlttmaf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xrvkkbqq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysikuqhz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qqrlcquf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikxygxfj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cixpgovr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2aqmthpnp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wizpgllw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jiwlvpji.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dzrplhpv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2rhxffnmh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2usxcmbtz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ztohzsrl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2oojieogv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2gznxyfud.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2thdzdmzz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhvtgkka.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jcptfksu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nylzlghb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2tpuljorp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2doaffhuu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2uemlfzpj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gbusfuxj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ugiekqyg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qxojnawf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2twqvaqfj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2rjmhaura.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ebmhnntg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2rdduanlw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aoihdiky.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qtwsvogz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qzqenclk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rjcuyyad.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2zaxsxdmi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tszdrnnq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zdtkfbyd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hmwbucen.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2yuqxpuxw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzpciytr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qrikdzwb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2htachood.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rdvpxnkd.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zcsdovcn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dtcolvld.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rguwleuk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wapnagie.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2nflqmbuh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vkvfaawq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vrejcjze.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qltbxdls.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2zfflyrvu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pppxeffn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2qvmjhhqk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2cmnrkqze.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lnfexbob.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2tvqsdmoh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxpydiy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2aekkethc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2mfegoxla.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2emcumike.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnxplzq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vzsxqvye.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpxdaju.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2stktmxhn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2zemfjzah.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2itruxbvx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gbfldlnz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qipewudm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fjijgfkb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tfdmkdnq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2tmxxgpnx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2yenjdznw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gfnrsupa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqgvgtaw.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qihbcfmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkujuubm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tesrcmbp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqsfzcr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ovwyfnsy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2biehjmom.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2efqymwbe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bfhhgzxs.html


<!-- 参考信息 -->