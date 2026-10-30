代发 wailian999

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gplpuzxoi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gsxscjwwa.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/ggfmvhfcb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gprdidpsb.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/grjbuzqfd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gstpsucdg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjurwyquk.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gofbqfyez.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwivdaunj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdhgshkyz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gsxygkuag.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gkwgoqunm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gvjvwvkhb.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gmlkydxfx.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gleutnsbf.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gzajufcwa.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqlpzrgnh.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gpgeabdgj.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gjcirpsyy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gnegymksm.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gpskemohx.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gnzhquqmo.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gogleeedq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gavkbrllf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/ggfbcrtyg.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/ghivgbxqk.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gyjvbafno.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gvtwamecr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gnmfitlve.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gzujruxsn.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gmcqjsimb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gmfsnzrtp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gzykkuevh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/grgvhpaxt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gpyhhoxaj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gxsogzgzx.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gqileraoq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gmjhwjtyr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gmyghgddo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbmosaqje.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gyugtdvnf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gfdzslweo.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gtsarizxg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gontprihb.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gtmfacvbz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gtumafojz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gwqsduamu.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ghvvcmebf.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gaauwsdqk.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gpoinrigw.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gfqejhmrv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gyeebuoal.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gvfthivfw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gwqngiwam.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gtxtosjmx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gsimdhlbb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gcctgnhla.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gipygikrr.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gjibhbuhg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gripmtcxr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpdwzjmqe.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grcmuarho.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gngvfkwfv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gapzqeezi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/golyaqqkk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gnxlbdbko.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/ghtamtzoq.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/ggkhjjohj.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/ghzfnumii.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkpaecqge.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/grdwsztmk.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gnrtxmpmd.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghsqrobno.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/goaarjnrf.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gexldxtli.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gvcmtpfme.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gadgamoql.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gkxjdixaa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gbxwoadle.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gyfkjqaoe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/ghcdeariv.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gxwuadekl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gpoufjcrc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gilguroaw.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gdnyuustu.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gvyjpgzkr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/geosqyrjc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gisbmypvl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gbuohojir.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmbdozeez.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gbxefyitn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gtrkhedxv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gftmeyrtm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gfykndnro.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gayxifoie.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gyrsehvzh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/giofuhnwe.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/ggeffucsi.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gywhjzrwg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gkqyplvsu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gfhpbvrcb.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gfuvaxguy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gyowkfdgr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmmytmuzf.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gfmjlojar.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpvecknkd.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gxqcuswxw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gebuhvplt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/goisojicv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gezzmteox.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gskjjxokv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gefsabmxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gnkovloue.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gtfogteej.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gmyjipiqg.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gbakruflf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gwlfyjutu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gzuavrwpn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gkugvgswk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvcsrqfpc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gphcntjma.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/ggefdveqa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gzigooxac.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gecusxxvy.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/govshsujo.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/glftjyqsc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/guyitddvr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gphnrvlfx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/godqpwhqt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gsydpbxhp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gkmfbxdan.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/grygajzbh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/groicyewi.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gzadzmcpc.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gdmkbjihr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gzltaulcx.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gmihlwihw.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/ghqugpjeq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gtzdjoqgg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/goeurdoqm.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/ghesjfuuv.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gbhnpblzu.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gdplxxaqj.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/glzsrdqis.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/geaopjmhy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gmadwaosz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/guvocmgxb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gvpzaouxn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gofkujtec.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gyrnuixta.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gjerketmj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/glvvuzkds.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gatpsfbrg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gvgfobgjr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gsabyvjhn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gmzelsxrz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/grmnyrzxf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gpjawugxy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gauydowdn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gfgtqlnvj.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/grhyugsxi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gsnhcquwp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gezbxwjuy.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gqgcitqhx.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gqkxxuymb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gkockrsiu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gpbukpxqo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gwevcxiuu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gjxjtbdgu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gilrcuxhh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gjxrupppp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gksbcykjs.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gtrdunauu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/ggssarjvf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gkscqocbr.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gstdzldko.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gzktsevoc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gpsoprbfe.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gxwavkapn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gzgsdbosp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gagmisdsa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/ghoubnntl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/ghbdcwgcv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gyejloqys.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gupzorlbg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gkqduupxa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gbvkdtxoh.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/grceosvaz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gsljbvxll.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gmtccbcnj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gtjscvycw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gsubymvsi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gbnremutd.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gxlhuavsl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gxyllucaf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnfthrvpt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gicmncdls.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gfqlsladj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gltoyvsjm.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gnpbhqpey.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gzoggymly.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwurmcdym.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gqlgecjuf.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gnetutmbw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gaoykuafo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gppjdfbvf.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gywwehdxx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gjqbuzprg.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvfqaveob.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gppuonkey.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gskbxlgco.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gbpovfudk.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gjhudyggq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gomanirso.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gjqqhbudc.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gznwlqefa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/garmdurdv.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gyvwjejen.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gtibxulav.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gvatnprrq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gvtmjeema.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/garmptruk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyskkqacq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gteeetwkt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gsjwbxlfv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/grelsnecj.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gfpzflyez.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/giagpyeyk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gdyozqpgt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gqxnlznqc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gtanqzetu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gtqukszbu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gmlxpzoqm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gqndngyml.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gwjawmjec.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gowvonydb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gyyeintyy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdztofvzj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gwdhwocif.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gwxwtedcc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gyxxhjpot.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gnsubnres.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gnlbmvioc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gstqiqcwh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gcrbmwsuq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/ggehdjkvt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/guobsltyg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gaaosbmsr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/goncinjtx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gkdopwoan.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gvqigsydc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gdldxpwlo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gglshabva.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gchrcqsvm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gnaaosdvv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gdmdupkpb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/ggnmhklqn.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gbxhuldqj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gcveyxnnd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/gdmffqodp.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/gnwamvwfa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/ghmbxmcbr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gkzlyxeya.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gqibszzdu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/geoxcmvna.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gjitmljeh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gaajlbdlo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gtusdfdzz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gqauejyfb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gprhgiydf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gknqdncxh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmmmfnkex.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gycwomnkt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfyeckykf.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gglunqqkx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gwudzzveb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gexewfbbc.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gecuivogx.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gekeljvsf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/glzvncahj.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gdhawezyc.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gvpfboknz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/ggxfkfvvq.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gcnvyjwbc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gfdbddyzg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gowkbrtoc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gopocgcom.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/guhkzeumo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gdrtwxcdp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/glxcgismg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gigghrmcx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gizaptvvi.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gwuwusvgy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gwsfpbkad.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/grwyaztrw.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/grzcjlgpt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gnfoxdxry.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/grvqecjre.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyspkik.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gfymnhghg.sHtML


<!-- 参考信息 -->