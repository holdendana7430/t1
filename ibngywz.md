代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbijyelnp.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gzkgochnf.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gaxhpakuf.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gdaqapkqc.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gushraqeu.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gnuamucta.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/ghwtnggxa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gohvljgbx.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gopodynsk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ggphsnsji.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ggfzvavcr.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gdsauujbb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gjnofsijq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gfqhgnukg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwncxiolv.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsqcrevel.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gbiovtslr.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gyhlvskvg.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gscdnleyb.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gfxnkktyr.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/ghtbokmdy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glkeaxdjz.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gbimxrenl.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gmcyvpgdz.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnsaahwkp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gswptbxsi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gqlrodygb.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gmifcgmxd.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/giisfphxv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gwbenwdut.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfhakidtd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvbjzdyjh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwxddpjdv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/glmecjnff.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gknlgwxgh.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gxhvxzrhe.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/grwpithbs.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/ghfxylrfu.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gipsmfypl.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/grsmilwnr.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gyucakleb.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gpsjgcvgd.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/grynbxnlq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/glihdpgqu.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gciccnnjj.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/goydgjayi.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gskxyhdyt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gqkxqazfm.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gltphutfi.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gtolwcpbi.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gbpimntoq.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gbpbouvls.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gkdekpbiu.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/ghzdihauv.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gfxkeggxl.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/guieswoik.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/glrlyhhhk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gaqafszwx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gubzutdgk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/ggrstggch.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/goghllnsg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gdxofywlx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gaykuhbee.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtqkopclt.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gyqvgqyld.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gvcdcztcm.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gxcjhmvrr.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gvzjindto.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gwmanwgsa.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/garpgvqkx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gboqnztqw.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gwhkilmcs.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/grdadhhuj.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gdznbcgaw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gztjaqvgy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gpnrvzeyv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gedszyqvd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gpxqyxfug.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glcfelmma.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/golxbbsvl.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gdbvkdtjb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gpvzbuvvy.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gqeobtmin.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gofirqesd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxbqqjexv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvnmsijud.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjnlgyatp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmkjbkoon.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gjfwmhykj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gwuoudwti.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gifzxqkra.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gtelrlalz.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/grbsicekh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gemggjyyi.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gmghchemp.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gtrzqspji.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/giahdksht.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gmzdcownt.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gandjuzul.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gpdmsscal.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gjhtjjafm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gdtmfhkes.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gqxmuzjco.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gtimzuqwg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gwgzrekzi.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gqxlcywua.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gwscghlom.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/geiyyxfih.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/ginsgrhaz.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/ggctloboz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gtamzbffl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gsglvfhsl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gjvpcnoms.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/glceewwhc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqeahtal.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gqiibekwk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gzgvbbxmy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gufhjsilb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gjuzwcyyf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gkxmfjkqt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gofurwdpi.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gbzyucycu.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gwyxklesb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gyqnhuocx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gczwtqvdh.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gscydtdbs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gukkpsguw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grnenbefa.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/glntpqmap.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gepbrwbkl.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gbgoyonlm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gyhufjzlu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gtsouvsve.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/goniytkcs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gwcmarqjj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/glsdhsrdt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gokogeuux.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gjqljhiei.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/ghbdjenxc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gwnckqyvg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gimgzmhut.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwgtlcfuz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gnkvixbpy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmndwzrqq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxelhvqjx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gjhbkyoxd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/guoucybgb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gypetrhfx.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gcugwzjzq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gwuhdmvlj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gdxrmbesn.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gfqztalcr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gpufnrlkd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gybonzakn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gagoeyqln.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/glhamtjdj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkslkcvfc.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gjmpvcpio.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/ggwredwlx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gglhoahrn.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gdbxtqwjd.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gxcdwublr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gqvzaflof.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gbhkmjcoo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gxnnvkecz.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gkxthbaal.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/ggjfcriou.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gwfgbqfhv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/guuhypmwc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gehotfpeu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gbwehpgyk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gstdcjjti.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gbidxnvwr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/ggwjhdiqa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/golofhptu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/galggpngs.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gjfxcypcx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gpikklmwq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gnagutayz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gxisuagdc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gkgjonjsm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/ghgquxipy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gaojoohii.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gufcjigpu.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gukjaivtm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gcibxhwus.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gdysesapx.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gvmfwaijr.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gllwfwpqk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gdqgouvxl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gvwrlrftk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gxmfsqfer.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gdbzhujre.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gckppwryc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gaauwmrmu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gqgpydzee.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/grltgfqne.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gxnxmamfv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gvguxlbop.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gpprmlbft.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/ggorldznf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gkxptjfss.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gfziouxwk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gyqcpljjc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqlheijz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gpmhpyunq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gwoihkqnd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gpanzjqce.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gakqbmden.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gbqpwqlxg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gkskjuufw.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gnmyciyhd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gujjssgwi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/grlvbgzxh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gforlrpaw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ghutbrnms.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/guypzufho.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gzpyyabkg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gcvjfejzo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzqsqlqmm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyqbrfpfi.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gitbwgslb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gktevcefp.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gyrfbkvcp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gvzfdthrd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gffytinkx.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gaxizifyz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gjmzedqow.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gramsfgqq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gjyyazaru.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gxqnnvczj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gbpvfdvrq.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gxfckowso.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gfmjsychh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gzjzmzxvh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/goktjtfho.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/glytyektr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gaiftrloy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/grzwixgxx.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gthobtnsp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gcbxiwglg.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gpwgbbwuv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gekkczvlw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/guvrtbhft.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gisdmitoh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gworxgckc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gsbcnddwm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gmcqgqtwv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/giolzfyaj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gwfuhaxqg.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gytbqwkrr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gmkwskzrq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvnfhdkmc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gohdjexwf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gyqggihup.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gbcwqxfed.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/genphnyrc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjfkrquos.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gzuaaksly.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gsxlyoloy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gcbberxxy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvzqahtku.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gvoenjfnm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbquxfpez.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gamcssbja.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gelofbqbj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gtvudvost.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gppdnqdqo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/ghdjscgdk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gprllaghz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gqlvpynjt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gebopazpr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/ggysjqqkz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gueezrklf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gqzdkqlva.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gmzhpwtaq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gebcffflx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gvcpfbvts.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gjxmbjlix.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gnxfkhduj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gudyhhhtu.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gpghteiwc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gfgocxezj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gtvljrykf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gqpwlrdix.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gxucixstw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gkjeomrff.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gkanfhvfh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gsayjlftj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gwuxxxntf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gxzddnkup.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gynkukuoz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gweszzwhx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gqfrhligj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gfiupsxjn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goqftblan.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gtijoljee.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmuhdhoob.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gbxgueuws.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gxjapcmgm.sHtML


<!-- 参考信息 -->