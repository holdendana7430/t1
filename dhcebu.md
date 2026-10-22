代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ifhizfry.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hftfumdk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qioyttac.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vfkmamuc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cqiyvarr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2isvohdca.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wzguzhyc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mhhujvsx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rvbhgidv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cayslmjb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcxlhwnm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcsjouqs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tuuwxlfs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zcanlfea.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjxphdvp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdeevxvg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jfhfwlwc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fadaezcb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cokzxjfa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mrzfnhdm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnrvsdpx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xctjbgvt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pgsrjsqk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cvvbtbkn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qffhgtdo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qdzwetpb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nmdlkbmz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xheahrqf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tamwtvrp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ccpqoabi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qcxqbtow.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2agjlbkiz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wjskwqzc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jqogxtwr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2itphfxms.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yxbxerzl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dbmjhrfy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aljmnrky.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nqvrayhj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktlevgpr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ixclrdrq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kifvgvnz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mbbfdixx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2endmczrm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nmoboulz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhnzwczx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sadaemvi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qgzmszem.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzuisfxm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kgaysiad.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2oriypcep.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zittjhrp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2myafvxbs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2upijppsm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uvlukqys.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zqryebbf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fxnxplqc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2aiuwgbdt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rsihxtsr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mmobfvdp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kxxobhkt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2anzbpbwv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2apsglran.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aidffauq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgiorqlp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2faqehygk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2romywmxm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvsewdd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gabcclit.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozcndeav.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2twnkljkq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cwfzinwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbcpiytj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zxexvxrv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdrgltmz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nbhfioli.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jninrumn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ylpaidxm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cbpukikp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mybuoyem.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2adgxhhnc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cqlnrepo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bttmsfvr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rwqittum.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bjflfycl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dkqmerih.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wvjvjzxc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pdzxdhio.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mecbabht.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ntfzopvu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wwjfxbxk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hvrapxkc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hmowmmbe.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxdedive.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2sewsgqgn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2iuvyqbyo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2myfkepyd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lxqmswmh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uknkqmiw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipbcsifa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pmqqxusn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xcxbufcu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rztltokg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wpzocsix.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jhkqftej.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rsekddqu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gmnntokq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2drcllhdd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fpjvjgje.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lnptkwlg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uqbvwerj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bhypsjvl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jcfgbluu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rgoxaknm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xraogtqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqythpxq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mjuvhimw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbhpwiey.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vpdnkboq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ndlviupf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2veolumrb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pxzqlkpk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqhzghby.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ivbuweor.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2pyrowtry.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2eaxmbugp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gyryvhxk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pnwshvtg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gxiljffm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vqgihhdo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pljhjmqn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gskrxdha.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqnmoxps.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nlmvrmhb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vomduxiz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2haybnyty.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nmwvawes.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qtysaqwh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rkndfilt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2abouxhyc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mnsctznr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pdlwkomx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ttdsreeo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2odhhkopn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mhrnooav.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2oiqugvvt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2xmosthiy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2submmsmk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cihqzszv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gowhiise.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2coipipld.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pgepoeyk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hztmpsxp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxqhbena.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hkajturh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hhotkeol.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kbygzwsa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ympyscfw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2beumijvj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suhbyiwl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hadandiq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2hzdpoacv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyesfwyq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pvpzgfme.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hcbjjuvo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hxgbigph.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xruyesff.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ayxtihxv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ueifeebb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xzxfoveo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rkorkvdl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2cnqywkdl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2brmlvkmj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2kynbqbgx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ebyczgwk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vjdearmh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2atbloaln.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2njgzvplx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2szjongbg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2aygqyfum.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ambdhfon.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pvwccvsh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2nppnyeqz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rgocqnet.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2gtsyapbf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fyxljmvq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tmgenyxj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uiyhrvxn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fxibzqsw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2tagqxbzc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2istfjxxo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tobtdrpy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2cmozvumu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ttklwcbl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pnrklsxo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2whubkwfs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nyuyhvlk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mcjjjutj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qlavcsuj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hlhdhndq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2joabnyrb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ykqhzgys.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kzykyewd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bmamolti.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2sjkyouog.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mgxnugfn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2fxjndnmu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tsledmjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehrxanvl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bqggbgkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdudbyhf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jxwhzjqh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vzvltsjj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rixvbpkt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2guqxtsxn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vtvosxjz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2zlyxtfpy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bbwnxsch.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hiciveuu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qmnypsnn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2cnzpfbib.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ylltmvjt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lhzzsbbj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ovaxjujo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2yxcgvxun.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlhwgwhw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmyrxjus.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlwtyzd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eakmxukb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ocptnrcz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2fryqtfce.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2cbdjgwgp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ilzljxbs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mlgyjoab.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jxuaqcmv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2udiwcxua.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zywtrpte.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qpftvhym.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zkcscebu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mddanjcl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rovsicrq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpocvew.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mlipnzud.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2alzwujnq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jnuytbgb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uvtivqis.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nmbsgwqy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2raxsdgpd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbwrbay.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2duwmpwgi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsszmyg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nvjjghxt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zlgteogg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcwzrmkh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nftdogbs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2aafmpjrj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2fipmpeum.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mcbemenz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2iotlhgla.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zxasbxeu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ciuyflje.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2moqkmzhj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2vyazojda.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jklblkny.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2snnjlzia.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2wcqpowbm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2qyttgoyf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xzgraont.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2huonovdj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vyghgzua.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2etbniddm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2mitwcaku.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzzsggc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2upjpnjlp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2arjptbdk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2gbsbarga.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lipihqhf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vnqupimg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ztbiwvxh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rqydoooa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2tnmajtdl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2agjcntkq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nefikzki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmkazfll.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2idbknvyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjebhtpr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tlqvrfcv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qbcchhxp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tqnhvljx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xbiifjkd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dqmyzhdd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2iijxqzdw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ebjzoupe.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2itzwmool.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2drjlvyjx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bzqnfjey.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xkvnxydi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kroawylu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2lhflhcmi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2tpqysrbu.html


<!-- 参考信息 -->