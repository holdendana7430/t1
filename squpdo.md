代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rczowcaz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2aixswmwg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jrvfxjsr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2spsquqhm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qrwgtcwx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swffsjmp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mdbzlccd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2narniwhn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vdnzmjlv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rkxmpxfg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hcuvnmuw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2noivewrg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ojsruary.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vovzjdad.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gtavjtza.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzsxtyyi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzebgrun.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ytndlonh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jsbjqztg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dsifcdqq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jrvcvgwf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2shwpqoyx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2azhcwhdx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2inwoysyw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rechwbza.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsixgjni.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qsiuqtti.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xrrualkv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2djazjxhy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cdshulpk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2erjesloj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pjsrwarg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zmhocsvi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vwbydkyp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vxmjslne.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dlupviyo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fhgxbyse.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2aeovbazt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xzoxgokg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ulukvrhk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zrwbrahk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oakbqocv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hefirccy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2efoptkih.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cghrmozd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tylsrpsi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cbzqwzkh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xdlavzus.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2idhbkqkg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqoiqzff.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vftubnha.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lwmitvwg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhetlhwp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rsakirnh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mvozwixi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocfcsqlw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gelrhdvt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aehcwxla.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tcpprntw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2insiyhvt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qsubuunr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dylykqsq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qcfjdwdv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ibdysetw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jretlgyr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2egkmzlzb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nxwajsll.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frrakwft.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bfspwmxa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2duaqglys.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynfofbci.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fivfmbup.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vjdrdgct.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdepasjx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pjeilssb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2stovuzyo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vafhjquj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2upsgyivd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywfqacbi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhfqqmjv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tunhokym.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkpplmuz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qvykjqml.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2puhkepuu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2niroebyp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vflvtofh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qtncqfje.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tcfymsls.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2egsublnb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2oykhsasp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vtmqfuxx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hszujjuu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2agnaitxi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2rpoyzexx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pvmxvlts.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bmwaxtpt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vnlgdtfb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxsytmlb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fucbonms.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zfhwqqjv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wkgpigyj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fydzcuxy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2giqerzio.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmrasfcn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kiafrcte.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jiknitfp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tfmsnbac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xudbhubs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yttmbokr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nxefiune.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2yfiyupbn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qquvuieb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xofefwop.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mqmnqysr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pfsldukz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2uqbxfwcw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2imddugur.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nrjcufbn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wtxrugqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzvnzhji.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xrjfuguq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyiigrnf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2eebhbkts.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nexlwhcs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jstjmebw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jlojijgd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cykzsnfx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gajqhjju.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mshvhkzi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvmemwyl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dcczwydz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rxtwlani.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tvfmapsk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfxkbfjc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oeokameg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kgcxouto.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zntbrinc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rujeohir.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vufuybbj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ojsfvxwd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zdgutwql.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rpskdnkt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bzrvjuqt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2boaluruv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qooprjpa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lasfrrkl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qneqmgln.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wsbmzdvc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wbxixslc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2gpumhitu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mtvrorsu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mhurebfj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltessnok.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wjbzlwon.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xtlasske.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xzvtiftw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zgifclic.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewgzxito.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kpljkdjw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2cpdoibjm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2yxicyjiz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkadxnqr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pzjwwnjs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2geyrwjob.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcnhlgp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ldfytfjr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiybzase.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dldpuyqk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fqhwiine.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mrlncqde.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rdbdjigw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ubxjvnmd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xnccrghi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hajecrgu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2gqdddfab.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bqxbfheh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lxykbyjy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2lnknjswo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2byjqmapl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2debcgorw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kiaycwjj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2sdmjedjo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bfminpel.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2snmmbeig.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vstjrmir.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nclfoirp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2durdoodl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2lzbgiojb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2fogxhhac.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rmwcemfb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fkfeqoyp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2pqvcwqra.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2phpybdpl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2rcwzwfwb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2yvnbhdiy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2yeyhysbc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yvszjmhk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2elusjshf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fdzfvbax.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pdifvxzm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2djbyynkf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dcddgqqb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2fkjzzohk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zwvexddn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2yxzyefzc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rhkxcjnc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gnbdkmpy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2emghckqm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2uvhuqomq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ewsnhshh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xozrvzro.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2anldnmrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjjmphxn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2peoqitba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqmvosuj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xipixmsq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnsshfcy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhirktce.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngucizte.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gqsdecny.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tlyxltxm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ymzpteqs.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gukwnmmh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zqdikaxn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kfzaihzk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbsnkmh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ffxmanso.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2nneljvyn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2zdzdcybu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjhxrhcy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlslyrcl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vltsunbb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2szyfkyqr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2vdnfiofp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mdhkrpqx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2liwdtorj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ouoqogwn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fpojiont.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kbtvpfvs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2mhvvoann.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ebgxnoir.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2cvfutiax.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2njxxsqrx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ihizlsib.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vqewmndj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wckjrhob.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zjyerdet.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xugcvvyp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jodgbjff.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2bmxrxmjf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2irilzvki.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xeabjbjt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2haporfcn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aebvqcuy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wtgqshvq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xbrwfwbc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fmwmebhl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyvuvlrl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lfrzjoit.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2itjhqqiu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zmfbyyar.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zlzwscrz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2mhsrsurn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2eskkzotb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2yzyebhwp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xompzgtx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2rmjjdgtw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jntllwsg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vrvrbtus.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2yhkebcnx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2eqduyyhp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2fzwlgmhq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2mgelbarq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ngiyjdfg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2paypmwxu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2uenonflu.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2btilfkqn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2bqorkolx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2wquonnfg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ffahggxr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hkfhzaku.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ieqhltyj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xdyamdgf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2chijxpgs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2mudbtafw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2owjetfss.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ehbixfxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzzjjkeb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2agednpuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rotztbqd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2txvtwwwv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2llhdxcvk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cdjazbrs.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mbqfiflf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgjrsj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lfydithj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2nxlxfqyz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2icfvyiis.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sfngidyp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lveppqqx.html


<!-- 参考信息 -->