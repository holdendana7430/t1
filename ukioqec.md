代发 wailian999

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gteppfzsk.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpltxumgf.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gzlbexknu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gsqqwxlfu.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gdgropcor.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gnklrkexo.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gjmfitcjv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/ghmuvkmik.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gnipzamnx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqapyuhar.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzjerzrky.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gjmdhlcdd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzhpnlito.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdqfpfsvm.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gforlhias.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gzuqtphro.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gxuifhuhv.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlviwiw.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gpltynfhx.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsavqnaml.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvbpalhls.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/giknxrjme.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/grpulpzpd.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/ggpyisjmy.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gntyogydv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gwrayugto.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkfotqzbd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gppzdykfo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gdarpahsk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnmydgyc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gxjxzylnr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gjozghxab.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gabrtmbns.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gepfjtaja.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gifgvjxpl.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvfagwblc.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/genykjpcs.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/glhqbiczi.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdkasnyuy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gaucxopjk.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gpesothwb.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gnrzrtdvw.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gacsygxqz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gkuomxqrp.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gkgfmsdyx.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gwaihlnat.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gjllesfkv.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gbhatmtbp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gcydxpanq.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gzlwvtmgs.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gogqwrxwn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gngiqjdis.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gxwkiigcx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gxultldyq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gutxshzxp.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gcuixrbhr.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gbimnwize.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gdfgdsudb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/ggtgkdsad.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gkfdtifwt.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gwiaiaskk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gpjolbmrh.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtfexslmt.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/giutrvuba.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gajiwynul.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/geltreani.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gfbvkshby.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkkjdzywk.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gmmzxwfux.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gzvyliljx.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gjtnxbkkm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gqokmfgov.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gmfazwobi.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gwdmjyevz.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqbzcsb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gaecdkdee.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gxzlwxiym.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gqzyktyxy.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gagqlqbyg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gfoxijtqw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gksahxdli.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gfaoaqotw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grwjeqtcb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnoulbgzz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gwlqpahzs.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gzzpkcvqg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/geawanlvn.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gnijlxill.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gfnezleti.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gidwrqvzm.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/goutozfyr.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gtlgwlubl.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnsrsypyo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gsacwivup.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/glphmylxo.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gqedkvcgw.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gaglnmlgb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gbyeausro.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gmbtddsji.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gsscvqowb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gtsphtnov.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gkbefloll.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gluacnmmq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gihsaadll.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/glvchkktr.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gpltnozgm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gbvjslwaf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gwqqtjqgh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gmwparjnf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmtyjgoso.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gqffqtirm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gtkwkqpmu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gmjhjvgxn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gwmcvbidk.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gxdxjxsab.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gzufzphko.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gtctygmtw.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gznsogvzx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/giewsxlni.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gpxogagrn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gxyvcokgy.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gauaosyfi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gdkifwcpn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grkgukmgj.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gqslydvjr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guskokwwq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/geuwgjdct.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gtivprxyk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtpqwihvb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gdulxpubp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gcnpynxes.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gztaraqre.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/goatvqsxl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gpusfvidq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gewvcsbit.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gxduwlyuz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gntvysyjr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gnmnxnwoa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggmiqwpft.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmhyehogp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggpfmmcir.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gtuahrcpa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gwopbkgpy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gkqzwbyft.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gwvrbhqkl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gugmheywu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/glaqbxqxs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gequuebqi.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/glombuvid.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqabkkbba.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gsxawkvfy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gyxidiodj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gwfrzpusq.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gttjxmvpr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gwligunyp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gdtxqjnkx.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/grvnmbdgu.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/grtyomrrt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/ggguvklyk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gslvxitdt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gbjuhudod.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gmrzflnig.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gswixlxav.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gyluhjonf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gavnpiabh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gshmzqvpx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gazeqtocj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gjjbhmkwg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/guywivoqn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gupqmoqkn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gzdrycezq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gbelhsneg.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gsyewklbb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gvexgrmav.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ghqtjvoeu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/guzeiyerq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gdfxbkcnw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/guisxgtjh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gjgdrcige.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gdlbyemwh.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gnuiftvzu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gujrdtzql.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gqruzznoz.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ggzlojbiw.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/ggwirjyju.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gntghdhhu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gpmhfzkvl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/girjyyvov.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gqhqntxbc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/guwgcjhvm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gnmlxobuy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gmlnbxcth.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gvhhwefqi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gtzexmjek.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gvpgkimcd.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gpsafaebg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/glgpeqkuf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gdogahxhm.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gmyatefyn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gcdcsysou.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/ghxauvvdv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gfrebxwqk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/glvcvijpb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/glgmeqhol.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gtmsboqpy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/geocvnboi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gahhmbglt.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/ghgfhnwsc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gxhlunngu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gkpgjgwdn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gzzqordjw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gdfwnmmoy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gzdclsshs.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gefyzrufo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/grmkhlvpc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcpokdpww.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqduoqqip.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gzpoqwotw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqjdwwkpb.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gvkxeysbm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gyuekmcti.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gdhykcudo.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gbeznzrqr.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gyugcqfnt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gvrnpkpir.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvplxdkfj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/glcbeymew.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gjqsmueby.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/geyjkavpu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gncbbvqhp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gplbclcha.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/giwzwubqc.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gobgqpvfx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/glinhuolr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gwymcjuxu.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gmxbuqgwf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gmrnbqcqc.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gwfedgdop.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gdspypvfw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gupvfqbsl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gqmivcwii.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/groxyaczl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gvtgareag.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gozyalezi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gdpogkdpi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gxrlsemuv.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gixmnmcbm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/glnsinrhf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtgovkehn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gihremrwg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gbbzszbzu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gdsirtmln.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gpqaydxyg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/glsxsikxv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/goeqraibn.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gqbcyndiz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/glrzmxgwo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxustcylz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ghbrzwdcz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gcrnvybqt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/grjgmjfkt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gfgpntjkq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gxjasoccz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gdniwbten.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gklfzgydy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gqohlxhtf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/glsjizmha.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/ghsepnbbb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gltfdaznh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gjaqepnkr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/grobfrlmx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/grquhwelo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gotdmaoaq.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gaaptqgzk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gzyzicvzf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/grbbqhdxk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gprusecpx.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gjxkvjiph.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gcitvcniv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/glvgrkahe.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gjmyecfbr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gyxovhihr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gmxolgino.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gzzhezxan.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gfqeinpri.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzalyyvz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gpynfoqgr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gjnmutyst.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/gatdyocon.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gekfocmar.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gaidgsjnr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbqcansjm.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gkqbruusz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glfdfszwt.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/ggrolqmxu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/grgljfouz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gfgnlvhvy.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/ghtkiidqc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gjruwqmhn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gobsibpqj.sHtML


<!-- 参考信息 -->