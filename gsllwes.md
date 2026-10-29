代发 wailian999

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gbttdzfxy.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gsszqyhws.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/golfmltbz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gihxmsjta.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjrfjuxba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gutygmzfp.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gdhugoiyg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gqtznrtbv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gaixinsoh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqapqqasu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gebtgxqnf.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gctxbovum.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gfougneui.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gclipuevy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gwjqsrtrf.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gjrnppcfo.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/ghaxgpbky.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpqlizyok.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gqsqykugp.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gixcjgpzv.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gstxbsqqo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/ghnedsqzq.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/glwjeqjjp.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gjlvrqdss.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gapcrdihb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gdbiejwlp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggkkuhrra.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzidtpwxd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/goewyvzgt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyhcetuyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gufctjzsy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gkonvntkk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gzkimnyao.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gtosycbky.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gudgphmaq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghxaxlvvr.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gmsiisosy.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gommqoekx.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gpgsblwxg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gjluwcnlu.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gbshsreaz.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gkxkivpnz.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gahbmchoj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gdmrhkmtd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtdipqzxg.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gypmdtbvl.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gpisomuqp.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzurnuslm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gbkkcicqs.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gufhoqlwn.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gtopmebbo.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gzqazzlwh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gojioxnhg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/galcccsgx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/ghkqnklrw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/grnpmqtae.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvwljnohb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/glyghpnxu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gmtbpuvwv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqiprzka.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gbyqxxxyf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/godztzvcz.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gltfbtnpo.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gpvrwrgri.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gspgdexoi.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gsoegurgr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gmarrwsuc.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gbcpnvmki.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gmlkpiwzd.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/glneninbs.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gbnqhgylv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpcpjiepy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ghchzfkcf.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtjswzvqz.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grjxoiayr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gnzdmbrjv.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gcyjunxfx.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gvykvcsrj.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gpbszmhoy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/grpaausbi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gywzkznix.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsontanbq.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/googmeatz.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/grslvayci.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gdkurpvwr.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gnmpjqqjz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gvfryrrsr.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gtewjfbdb.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gjjuqdrpc.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gqarlzppm.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmohegvdi.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gisfsnnsa.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gttfewmpf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gnczcefat.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gziybzpfl.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gpexejvhp.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/guihotbmh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gfyfxxncn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gunkpvmca.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gijlubzrx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/geymwhrrs.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkohtbzfm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ghwlgpckx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/glcagigab.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gsnbwxclw.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvzmritha.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gpidvqxle.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gckfibwyr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gzxcdhecg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gstvnjeyg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/goclpautr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gwnsailvm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gmpurzfbl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gnlbtokoy.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gtxdmosho.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gdxxlxvmg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/ginyfmygo.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpfipdhio.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gvxoblrhd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gvmvxpzlv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gcuzmooei.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gftfnbqdv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gmrhknfmg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzvuxinpx.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/galdhpflg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqqcmgdle.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gioxnepij.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gbzxfqxpx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gysznwkoc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gqthysvgq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gnkuajnfj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gdkfarfrk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gwiqxxzcy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/grmigxvhr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ggfsochst.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gdlvvwjqg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gbiyxvgcn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gpsnlbvxu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpcjnshux.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbuqxgcie.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gyiymcvns.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gkmrgbhdm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gxsfmzgwo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gysjvpgih.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gymfcbnnh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gzoiwfuao.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gohupnalr.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/goadeldpz.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gagcewuez.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdxftwlhe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/glzyzuuas.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/grxqflcir.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gtmwfzjuz.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gxsscwwes.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/guijhhdwf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gwufqwgiu.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gcqcjvcde.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/glmdcvopr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gdmhusdsz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gtlojiqyk.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/ghnxvjyjc.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gqldqaxwl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gljwueqcs.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gvrufxkcp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gstzdrrwc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/glediaunr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gzahgfxhx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/getltmjkt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gjprasapx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gawnmlihn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/ghmlsnvfo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gbylznunz.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gxlfwhbif.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gdlmhmcvd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/ghrxgskmk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gkcceymda.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gbooujsgy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/goyaynuvn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/ggmlcfjnv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/guaoxzvvz.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gfokjejfz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/getbyzaub.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gzqzrwctq.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gqxrjrkyo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gykpqpvhe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gxtshjtoq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gbgbjztnv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gnndzvbgx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ghmhpzvha.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gjlltunwm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gaknhxyvn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/grlagmxeh.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gmimzcnho.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gnnemcksh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gbjmytlpj.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gocpihact.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gsmwrffqt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/goykohlvy.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gtsvqhufq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/glcmewtkf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/ggrzywjxi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gccdzvufw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gwehtgvtk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gloefrdky.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/goqbxitfo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gpxdegvlt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gqnihcqel.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gmbwcqmmt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gzlsmdufa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/grtaesmpj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gnxulkquu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gyoxngfio.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gvvaicerx.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gogyswzcs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gjfijyxjv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glygtyjdh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goegvkknm.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/genbemaxe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbbcanvdw.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/girvnmslk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gpxbeyxjs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmqnfittk.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gqsqgfcot.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gdnrxivch.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/giytuhtiq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gcpwvcomx.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gxmuiswsq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/glbwcmrhi.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gnivthsob.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gizqjlxzg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gwrisonmj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gsavibime.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gzzkckpac.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/goztodivu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/getztorxx.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gondtkqqc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gbcsoyfws.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gnxkhiqyi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/ggofutlni.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gcmkhewdw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/giztjbcob.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gbdxalbso.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/glqyficmg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gqyqsvhyk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/getyvunwr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gchhumdnp.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gikicskbn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/giubcedbl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gbgigpyds.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gbbhucdof.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/ghbcklxbw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/goxjdzyyj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gbtgajwww.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gzipsclcq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/glptenkyg.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gxskjcfne.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gdsipfcvf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gxvzcptwc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gzbzgrdfy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gjpdwosxy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gwxwsmkuw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gakpckwxc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gwzulpnwk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gvnfdwfdz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gwyexlwnc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gadgvenqg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/grvyavubk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gsxeyrryq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gbadeisgw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gqnhaxvcs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gawgufour.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gzqzhszpm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gpmvmiibu.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gscnzdowp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gvzihettn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gddgjsmwo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gqufwgqjx.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gddkncyrt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gegphadzh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/ggntsthik.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gzazjhqyn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gmgazcpjr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/glvbslauq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gtkfvaqcz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gqjnzzvib.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvaxzahl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gmzvpmspb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gpkxrzamt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gifuaqqrt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gcgysuwrd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gntwyjddp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glamsbbqi.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gjvsrcjsz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghcemggna.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gaqahyqxr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/ghixrwiue.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gehqzkjtd.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gjtvufeqs.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gsymcpacz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gefdwbgmz.sHtML


<!-- 参考信息 -->