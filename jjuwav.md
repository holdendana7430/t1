代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mhoiisrz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dcolsjbn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pydwmhdf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rvcqwaca.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tbuezgpl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qiumoieq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2sldsavsp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nwqpwpuc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wqbktsns.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lgbuuxgu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dxlvmiqy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rcuizpws.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dicgzcku.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fannxklw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqxmhovr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ocmvdfet.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lmmuypzn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2roevznfv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gtxkecdy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uxwqteyy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2blyyuqko.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahyrvmvi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksluiviv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2abvygrvm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvlajdlc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hdsbtubs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kfujzheb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jotrhuhs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2efrsmxed.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kkpdwoee.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2waxnpbfx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ddltzbmi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tavzriih.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mxurvidv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xyvmzjrm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bmlbxubz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sipfufaj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vtqdroif.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wkdgydzt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bznyfxua.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2suojkjpx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tldgvdex.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2esqeylsb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qorkdcqe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2voruvwqs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qyocvkuu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wppcgpsf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zshybqbk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ozzxgugi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2psopaikx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nkfffzha.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvykkyjc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kplnamix.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mopkomyc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqgmovil.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pxanicbr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yucrttcp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fuyykbgl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zxhtxuca.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzmxpxvx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djkcjboi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vecvolca.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2firlaizg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvcpgslp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2anfbtahp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uuzpgcbq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ayecypno.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zewpeqsm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iwsmdwoj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cjpejlny.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xjeffdfm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2geszeyfx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wwunkkyb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mshavofn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rnbvrlqf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tipoljov.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pthsmgjm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpgbcwxm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asplpmba.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uyspiadf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2epqsvfeg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjnqquij.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2exnbulrl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2svtrcdlo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqemjgtx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tlhbhyjd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyimuiko.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2schpigyg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zzbpwoip.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zlrbrtyx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wvhwuqyc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2auqtbeqh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mdehbmlt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2egzdwkqv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tuxjqwnt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ivjkjkos.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2omhzbtsw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zgbcbnbn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fpoqejxr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qszaaykd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2yqxwyuwk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yxvcxzze.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wfcikxlp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vwngsfkp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hhutxcvt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhojpeop.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vrmhiuyb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ylktkswx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2eqlqwcda.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ebfxkovy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcdqzayw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fzcfckjt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vpvhwrqq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vxevyivr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jlcbgxso.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mbnnfztv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2tntpeyti.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ckbfmnkh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2odutxtuh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hltlzqlp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2udhvnxku.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxxitjb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2boptkhnz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hwexdcpq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2eqiztxoq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kvugbiil.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tytgfxev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwhrlxqf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2izsyavzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wohrccwt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2csjlofzp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ocasvmbd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vpmmfrud.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrypaudj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2asvmopur.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqcxuegg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2epatuelo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2acnvtfde.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wbqixoar.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zddndgxf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jrajpwwi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2derqqbhc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nrjxkdwx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jyyltvkx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lszzzhuw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2bsahvmnb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cgetlbzd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fachwuti.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eehwpqpi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qnbmyjrs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nnkblnps.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ocosndmh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mpfwpqfj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ybqicgos.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ztwdrgzj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ryisypfs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tuiasirp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ggdatefr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2axvhmasj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nkczgycr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2waimnxps.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvlccbiy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hldejnsi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gjahwkzf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zeicbtxf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjyfvhqa.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vnlyyjyv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2uwkfesxr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qzzgpoln.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kkxequzr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2npeexvfz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cgcmizmp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nazcbqya.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ycrdhgjm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmoxniza.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xeemedml.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jaablimv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pzdzuprr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yapzzxxw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2usgeybmp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2eydmqueh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jqcjhneb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjsmzlfn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2swcvzrgo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ethhpdhy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uswjsefj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mlupgbdn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vimlewwg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2orityvbh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rulirxgo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2eigcuyfh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2tjvsqpbj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cytshijn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rqrgvzbn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2remarwif.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2omkvckxw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2eqsocltl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2fbhgfukq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2kitpqpvx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2okkjyflc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2sekmahqc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zjfbotoq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pbdaiegk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2euglaasg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gimfzzig.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2tukingrq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2evlkiuvn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2opphjhdq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hxmtutsx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uphawenk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2aqvlclkz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dezwegec.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qazcgmdl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2tbentaax.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qvjhajbi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qwyweffc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mcgzcafp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fvcuyszg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2nxmfsram.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rzdysjii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azkbcwuu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fnfymbfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hubzwlpe.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eqebwdpe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nllwylju.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mqsiwhrf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2saobmxda.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gwzkozpe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tebudrsk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2maqzdyzy.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ehdkzzcj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vfuulngd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kfbrtjkv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pzckofzk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gzxtmpcn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qijcljwj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjmxqaa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ydgfpmmt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2szbxkgwp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfjnglv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fmzowlnq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2kbtokdyq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujfjdewl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2jdafhmca.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ykmudkdp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2knkmduws.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ltorifpj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2xsuewbvp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sthzdbxj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dxzmmjli.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2gsvbdmit.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zskgdlpb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oodbstph.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lyyorjez.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2euhigxxf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ovohtwjk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2woifwupo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2blrmdkvx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vjcpgztf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ygycdtky.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhotvaxu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gnmcmspi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ikprwvbp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cdbeiskm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2tyrwuovj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gnsjxmeu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vytcggkw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oogoplio.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2mgnmanaq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tmociauw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bxnamczk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2syqhcgyb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2loxdztug.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bcbevrnc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qfvyrtcv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2imusqpuu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zcahpsap.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hgjgorjs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wbrroyqy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mpcdqfbx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2yikyurnq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2qsiwkrrx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2hlghzskq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2umdacemq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ggezqcyj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgqslye.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rbooldot.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hpvnbrho.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hchpmaho.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2aqjuidvp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gjfobawy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2hhyjkhfh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2hxhpyhii.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2anhiqeua.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vzdmogkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aphcyznf.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2afwuiklb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuozkefc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tuelursa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2jwgczdaz.html


<!-- 参考信息 -->