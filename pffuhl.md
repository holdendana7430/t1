代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2avmmvioa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bypaqhyw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdumbpi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2elrizsqe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guykksxj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hfffugcz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eufwdvzd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2chilfdrv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vypezfhf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wacmnziw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ilpvgavz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dbqwsfps.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gqdpocsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2amyrzwzg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yjyhelwi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pkvicgqr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2seyveuyp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tlvzzzfd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ynwpwosx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ddidwzms.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cxasikie.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2onpcvzvn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yskfwjns.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gyaodeex.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2akibancn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2njcwxunv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2orkqcgjv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wfivciuq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxdsvvnw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yjgdvezg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vcfhzcle.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nepgbsxh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ctcxvqil.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vxrwwcyj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2slbcdnwu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvmtqzpo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rvlbjwju.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2awawnjil.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mfbngsrf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wdyqdsfa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2phsqkjdj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2itaxoqjo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qgcdcsij.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gviwqmcp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ofaomgzw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rxhkisrx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nsxquqxe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2niuwjvae.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2biichjxd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2seyrzcfm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hpvolrpy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qznskbna.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2llwjvfpb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcnpatbu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gkyistbo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjwjfmem.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xlyahwwh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2holuyvxf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqfzshne.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rufqulnz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cnwymwlf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rgrgyihq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hukalhnd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lcfxuwnf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yoedfngs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mrxobzei.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ucdusdej.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mekttupc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pgncodxf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2slgtnzrr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2psmijzek.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fnnkbliv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cnnfxedg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oujazdpy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tsxsxxko.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tylxqymv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bylaxnzq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wvlkqkzb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2poaxowyp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nitzbrry.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifbkdgru.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kclifrgc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cgjecbwn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vekiydkm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jvayaehl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ngersuuz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lpgbpsbh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2urgmqucf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ihojdfxi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bremabfl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2corovofd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbjrhbdj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yxarjnja.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfbyyuaw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rluhdmnm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bnxqcphg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dqojimai.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kwmkqpcm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2btrnmnbk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2chxwnsai.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ehfaqezx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2bfzqfgkk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2projqbah.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tpvfdmpp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vzriqnjb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hqpprgwa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ngpixoep.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jfaijpyr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cgormdje.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2brnaactd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xunxuqme.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lgrblhzn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ywqdngxh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2libfhxga.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2diktoubs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmhmdljx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2oyvprswu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2efjgrrri.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rwffbpxu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2npnnwlvd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nwzgyxjg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wuyrvgfz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qwzmlaqx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gqfvitdo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2abiitwvg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yodsaleg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tltdltbv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fbshmykv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vvjgnjyc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jxeomwbq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pgfzzsbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqgmyiuv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bzwfkkqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjlvccnv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2srgkcfxa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqbsuru.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gnexrkmq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ooxmvibv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqohrrhw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2potazhwd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2khnualdm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yhrpldor.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2unpakkey.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rfieikrp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ppcwfhrg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tftdyqoh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xqurpuoy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2agqlhaex.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tninkxdr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2khwbmgec.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mwednkvf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwrsowdd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vwqvzgyy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fyvhwrpj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nunatyhq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vlptdurd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cqbrjuwt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gafxmtrr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2umatfxhv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2skgozble.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hkqeqzwg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nshroydu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sxtuhabf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kashmjrp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2arfhszxl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uymlazcg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ckhcxxkw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jwyfohzt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jzdfoqse.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2woumbvvg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2daalehgn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2itrnaquu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2naxcmdeu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lckdmomo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuldbkas.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ykelzkal.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ltdbtebh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rnwytzyx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zebpfbrm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2irjbphyd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vujhmdon.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qusyeopx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gvoqfxld.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2edavfivl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vktkftxu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cvhppxvr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jaryxgxe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ulonxafh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2pfkzilbj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qhdqwzwm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nocsiuep.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2laidnumx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ocliugfa.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2clgviywg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2deegqkqt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2aoubkvpa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cdvycazs.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kmuzoqwm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wknarahk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pojnigtu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2uvyhobfg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vkrncmco.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xevuivsn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2abjwgvfw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ucrscbkj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ixzqwwyr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qolkvhqz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mhuhwxef.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nrbrhcrw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2uptiwckw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2uctzwebu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxhrdfbs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2smsdqrbw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxewpti.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2cemorjru.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2lqakecuf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ogycowah.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2slooafad.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2waiuwxno.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zobumynh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ycagnorb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mynyjvyp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vheelwye.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lkdsxvwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udrxnebf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rtikgcxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxzigcjt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2lsejfywm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvosnnkg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pivrlybl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chbinsrm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ldpzijyx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2kwkmquzi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ljiqefsf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qftwzeyr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dwzzopos.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jvszpnzp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dmpcbeyw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cpuurkev.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2eejvqlfe.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2qpyjcoqf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ihdunnkp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2thajodqs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pmnefhem.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwmyofoi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xgcyjktq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hugtluaq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2pogdawvk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ymzebqie.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jgiznllh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2etipguii.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2tioiksyo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2feypkjrz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2trtmvvjn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tdyewsoe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fayjiqwm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbtwdzzm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dquwpwwp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2teuedscn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tidihhwv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xpknvqzf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jtpodfsp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dkmizugm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2azihzyiz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ibncfvyc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gytakjtj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ngqhhqly.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwujfgi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xegvxsrr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2oxkluzey.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qlrmlexq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2xzipqzki.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2blnvuurb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xrgdpnxe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2cooifadh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gohmiqah.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nyiatuav.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rcxapjhl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2qycikqmv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rkfecevr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pcxhykdb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2htziukpn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2vwejmldb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ljmvgoma.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hkimdafw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2bzvjaryo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2uzpebuau.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2cawljtsr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2kmndmoxa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2bqotfmnj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2xhddmnkb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2qexcouml.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qxkfvniv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gagacuyq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sommvcfr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xnchujth.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2hauowgii.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2bffjaemj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2lraxsncv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvaohceh.html


<!-- 参考信息 -->