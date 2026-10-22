代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tgtbmzit.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cmqsbhxw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cyfoidmm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2melrmmhx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ttpjkpwo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gaqtwneh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ysllpmrf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mfmdcwom.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oimrqtdd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxowhpdw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rxcldpct.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkgilvxg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bptlggwe.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sxzjgrgt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rjnupvwr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wiyulecg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zexmcgto.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ersxodvl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifvywjll.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2trrcdqwo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2awxniafr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vszqcfxs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rdbimdta.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tciajain.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ixykfrlt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hrdughru.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iwaojjts.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcellgql.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjubungt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lbfscthg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hvznnyju.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdvknevs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mcjvgoum.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yhdvztlf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sstmgvfi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2swrwlkdf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mpeuhyff.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2igeetvxo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dnqujyox.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nougbwjz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2okonknsv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nkoyeazk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zbuvqjnm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ixijenaw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wisfhfet.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfncwgrh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipoovfdp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxylenyl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2kllkpoky.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwgkjgrm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzppfonj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tlzecaks.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fadxyigz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pxfqwtfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2peznkgzw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pqfnebqy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqbklcq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfaoobgb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ccahgnfh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svnphslj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ojhfzsoe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qxodmglq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oziwveyw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jnxkkcku.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tkhzthsk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gkmsiioe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ptnkkymd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vbxdpgqy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pqetfobt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xftadwfq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2keamqpak.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgxxeyv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzonraty.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wruvllch.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ytlopnex.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pgttpyom.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gjiecowa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mtdmwboa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2epkojjzb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eadtbboe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlhqvhag.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwezyumk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqxeeycp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uhntsjzp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jlasioqh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrzuittk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vwnkiasi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2aotiypnv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hhdywgvb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oixfqdbp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pfughfic.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zhfuaxmp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ueuzznwn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2altqhsiz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wfeoqrnl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pvhmvewg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rkdtvrfq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2glmaduoq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2aviyxsyp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nxkmbkvu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cthnochw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2esvmbxzv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mmvwutaz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nitmgoly.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2huiudjmd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uxmoipox.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yaarhuva.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pgyuwmjs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vwprzhml.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ycrjvrdo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xxmifqhl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kljhcllz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tmedyzqq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mmhphhrd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ckxozrpw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2syjjppkf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2atzgjows.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mtpgyzyv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lkzytccg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qumainnm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2birahihz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2skoxpliy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2unvtjmkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvvfbnig.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vqofpdsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piupqprk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qzqesqvs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmeevev.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecwcwwms.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xjdblneh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztprqjhm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nwkxahtv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kjgrwmak.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuugyogu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xszlsela.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2blbdxdzj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cwxzebjl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bkskruqz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmlqktpb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vlpypkux.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yskvflfq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2shqicjop.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcvbfglt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnfgvuug.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zlyybxge.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kobjutpm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2crhjxazl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2djhrzwwc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yolltiyn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nscccaea.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nuhmacyu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2blndiuxy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vqfeisek.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hpkbaqdl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2almwccpr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wdzvdvha.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxxacrgb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxapaxfb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrwuenan.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vvdkwnpq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kghwodqq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2tcymneot.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xztwcmml.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2aaedieew.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ixczxoly.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujvjypml.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ciszoune.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aahkmcls.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dacyhwon.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2huieudfv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqsvvscd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vvzwsoih.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bzdixpcq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2urbgkzgb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2umaaewuf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2boguwzcr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2itewdssp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2icpmtrfs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tqsgsytt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jmzezptj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2csufdfgs.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fasvrpug.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffmxvjkw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uudzsdrw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vadlqemk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dzhivtjt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mthhqugy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2unadujrh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2avymfnwd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ebegabma.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vbhyxsuz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cbdtayww.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2udjwwbxu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wljhgrwt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kfhaezcc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2stoznelp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yafgewxf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2kawejohf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2dxrpuusi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ocjmuhhd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wcnalicr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2rfuubihi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jfobfbjw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvbcpjzw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ctnbugzn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jobxfrox.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tjwpozwk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2pfhwpmtd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2sertmjbp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2afgarvie.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sxjrwoit.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lhjfuwlw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2uuhwsxuw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2svnzwigg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ljgzqoqr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apxqkmkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjprjetg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fwqtyefn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvxyvjjs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jnvbnyum.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2akgydrpk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yyarkpjr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjpdaqe.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqngocvp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tfafhxes.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2gzcqosgd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kiebsgwv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fioqbdlg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2guwjnnii.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yrdpttwv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2uqutrutg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kfprgnli.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ndvcpcvq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwsrndng.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ikukesfj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nptcmcdf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jzlmolwe.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ogetkncp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvyjqzya.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2meumkeox.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sooexkyn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2txjqvcfp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2dfidbqej.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2cikvobbf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2rwakuwky.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2kdwlyrlh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bokbxbzz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bxyvdbsp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oqjwjfux.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mvqywiod.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bsbbmffk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zackawqp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2pnoycyhk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ixtknkde.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ktduqsyp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rtqonzcu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfogwvbh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mryzhmio.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ynvbhtfp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhiauvw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2cssicrfx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jhxeyvzv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hlrfxfvt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2iweeslhp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2tnjotfil.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xufejxds.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2iflghzil.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tdzefdal.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2twwvlrmn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hjsbmbxh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2sjysjcmp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ehdnvuhi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2webvbjzv.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2cjbhagvw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2twqqrzps.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jzhnwtxw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2jdtfvdcp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2pcqmejmy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2gmafbjzq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2mthmkfzh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2uwtbtazw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2cxxpcvlg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dzjookpe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jwhwjbtg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hsmjlpby.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xqldgzbk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jjptgmzb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fmdptfxt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2vjbtdjtr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2pcseukbr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xmcsuzhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvsetjtr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2udmgrkoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opuujgjo.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2zppxglua.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2hpeoollx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pgnkfpwd.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xhaqjedf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vhriefgf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2aewuulav.html


<!-- 参考信息 -->