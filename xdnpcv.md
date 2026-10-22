代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wohsjwvw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qvmwsocs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xbttjzkj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zzhhrpvx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2spoagflf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phbzafeq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gdausbzv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gnxpltqv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cvoaakhj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tgekbdha.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2arzbpqzj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2cneckccx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ezahexob.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2phkbzihw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ukaulcel.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pkffwonh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ffijpfxc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2grxoeczy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uapnlnlu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2powlkekh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mylhhbyr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2icywccra.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oslwjrln.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ipeezlbn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iujijvuw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avutcppl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ppeuxpoy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kchzhzof.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2lronhiwt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ncjivaoz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2plkitqlj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dqfryiny.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mnvqbhoo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eaealavl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vwkkwgfb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wrofuodu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2kdurkcyh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rstzazhr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tdcairgn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rhbdsgsi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2anwfedre.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjffnpal.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhdvzujz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2obojxsjy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qpcooech.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zrscnygn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdcbpnpb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2udtworue.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mlnnqgoz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nlrahtwf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lkcrsnus.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jokhzyvj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ansujghs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qawdbnat.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rhpseijl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2shabrxuj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2shzpktme.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2exvbaego.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2egjxcqrd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mmbkyazs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hsgletak.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qsndsbdc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oqfgxyui.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rzdyscgp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qtdlyjun.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jmmcsrir.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ppktttcf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uiudyiae.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2heauwojk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vnccfqvy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gnqlteyf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bkutqqcf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pwzjfkhu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2szbvobsn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvregsxv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nhqvsjxr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rdtdlcat.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mierhbpt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qplatkyr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdaxcok.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ljhgzbgy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vewpwlsq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rurfmfdq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xthrhzjj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ycpvizch.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2giasijvj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2adisvpab.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2idsyeojz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tcelybig.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tbltetri.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2huqmpqhv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ahxarclo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jvrlgsnm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mfyblvkb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vblfhitx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hairzvni.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vhuymtyw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pzkdkicn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2bfrtgcbd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fkgcqlly.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2artzxpeq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qoaynepi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgzvohcf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2quorvudj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nglqddwk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xlyifuvo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yedpilew.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2juihbnsh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bepldzmt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sqivjpjv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2muubjgyf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2syfstydy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pequptpz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjhozpuw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2unhbhyoy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nexcpxpj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2iqgmfhyc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vsoataaa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2szwasbfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvglsqmh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2mtxtradu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbggkzha.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zulgzoai.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hloysomb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czjxwpgj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2amxgbdrl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2frkptmvo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hazmiqjb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kzsnoufh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bbwahcma.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmueaxml.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wlslxgys.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tudpiqcs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sttrlopv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnhodckz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ufmcziyj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plupfxse.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xdbggpdr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqubdqbm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cztweuuq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2unaukrfb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2nhtcsuxl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gyqraugb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aknknffx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jxlcdfzs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fftlkyga.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xudkhnbx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bgcfxtds.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dczcgsrh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2eopzphaa.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2otlfxrsf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxyvqsva.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2phnxqcef.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ujkhyzsu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbtjoyec.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2soxcwdjd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgqylckq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xnpahify.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2aagynhhu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yzdrfypd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bfognmpe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kkurhilb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egrwzpha.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukgtbdbf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2knvdxjun.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wbvstlst.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rkmxucxr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2irbabwnp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pprjjtrm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kxrlehty.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ovbpuuju.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bgyslpgo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cobahdnk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tcmkglbm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwdyocen.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wgspohkj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2azjvqrel.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zdupgowt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tbdczlit.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xlujahij.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kzjjpiej.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mddikizz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2andihhrf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2zmlfnyiu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tiexmmuj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qosrtoaf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rjtkpjit.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xzrransw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kjvfnjjk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ryzlligd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hqzadwtr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2kyjstchw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2piuiebqh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2fpdruihj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lrjzryly.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2gtffiqhz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2riudpteq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lsymyacn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkthvawu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqxfoday.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uokpxpyo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2mhgspjoi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rpqjsjxy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zzcfiykz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2reolngoi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2vrgrbthq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nwuaxzbu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yuzgeadk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2otkbxeym.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2aujrrnwh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wnduxfpn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mulywwdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qepmigkk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2evnpwkbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qopappzf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zwzipqeg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvqmphw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fzgcvypj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xnfrwykk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2chfzroeb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tydnbknd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wxydiaof.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mfruqonr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ydjstltn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2iboeqwef.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjbvoeh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lcptxexk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2uacofzgh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrmihmb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kmwipgfi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2escdzjkz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2muqjdigr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cftdnsqd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dcuafhmk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chawqyhc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2qoyssztu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ttqkradz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2stifbhbp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rnzegbyc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2njnzkcaf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ifutsmwz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2brglesuj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2cozkubnz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wmmhfukn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vnnklekc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zibrwhdr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bfghigyj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2phwayhlp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tmeecaek.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kgpsoncm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2arinbfys.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2taksscgj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ymzdpomk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2baxuqhvt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mqwqcswe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2stswehum.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zhuscgdt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ayphbwsx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zfwathuh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bcgdcpdk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2qdjqauve.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yldwisfa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ohcghaql.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ofsqprai.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ftxtxyvf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tkjtxfaa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2eptsuzwq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2qtvfmfop.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vvjmrmmg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2tydxrjfv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2iuldgclx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2fqibctcd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2caneomlh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2xhxmifqm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2qgeoqgmq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2enmquqtk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2cnqrujsu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2xtykfias.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2usdqfhwk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zjtpatfd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zdxbnnet.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iabbatju.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2panwzgnb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2vhaltyyc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2uavxtytk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wpbkthoq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2vilwsqsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duveorab.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2yamvanaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpgkemlf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qljulzck.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrlbldq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2isduvoby.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qgmjmgfr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2upufzilh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xgolttnm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2misqhgvw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2yzevyets.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2jntacpsr.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bspizntc.html


<!-- 参考信息 -->