代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gsafhnlsk.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gjgghmarj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gqtzzklod.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gihdffxhe.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gxjtmthcq.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbconaytm.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmlekzuyb.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gvpbnkuyc.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpbziuatk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gupddaizv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gdogzllwj.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gmioufygf.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gcaihckjx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gxfajqift.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gketjhuip.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjrvdofc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gyyewonzx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwktdinlu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/galjnwkel.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gwzzvehjr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gbrrzuyyf.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gldhahpya.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gdxfqyoga.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gxaqvtufu.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbdyrneik.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gbkcwcmks.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/guijavuam.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gkjjlqujf.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/ggmnylneb.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gnvavhynz.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/giecpbvvr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gvuahtuzi.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbkaupgnz.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmykrhsba.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/groxbjucz.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwyhqgvpf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gpcyeolqn.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gwqwmweuh.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/giqdytjlm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gwjwyttus.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gwyutudsz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gxfjxmcad.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gxeeshykp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gdooueoxa.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gesqplzcp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gacplyydn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gepiifyyz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/ganphsflt.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gqmzhmmew.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gorafkgwg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gmmaqykub.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gvzyhlklp.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/ggnlaaxgf.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gywiwznqk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gtellhedm.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmpjmftme.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gtbfocaib.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gbvhuokes.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gptlovpag.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gwtrywcxy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gobxtnecm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/ginycpzue.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gzgeyldea.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gayabsypv.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gweghrged.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/ghyskzuvi.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/guaqpdgkh.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ghrchkmut.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghufxyenx.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggfxekomj.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gcearmcmp.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gcbfkyagg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggeeeutmi.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gstwbujay.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/ggfjjczvz.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gogpbznvm.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/ggqqcuhha.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/goetcohlv.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gbunkrssw.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxytcavxf.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gplwqmkuc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gsgyaopum.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gdubpknwy.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gdgbclsne.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gvvqaeviq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gawtigqej.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gwhcnlcnd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gnqvudkrp.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gfbfhtfxd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gqmmiouwk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gjfiblkqy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gprgcnuif.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gluwoxuqk.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gmscgsycv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gsvpvbtde.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/ghxuiytrk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gahbmctjc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gcfbmsbxr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gijfbukgn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gjvngpdgn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gxyldgmjf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmfivwnsk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gztzlvcfz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gltmzyidi.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gjppcyamg.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/golbnfnmp.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gqigqaibf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gavvtfbld.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gosoywakt.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gyzykxqsv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gncygohuk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghumjcwre.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gphalymhj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkdqdqyeu.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gzbfxbfan.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gqrzpqtxp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gvawfasnd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gguoeavnl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gocheagsd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gmejlkcpp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gfciwswbe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gkrlkvknx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/glwxhhkwe.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gyjfclhhs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gonoarpbu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glybrktdg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxygrmhcx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuendade.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnxkqqqdp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/guubtkpzv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/guversxzy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gyjwppnap.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gmzhuqbdm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/glkayxwxs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gzrmuhdnb.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/goqpdhkss.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/glbifteno.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gatfpxrsp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gerwlwthp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gocdtibwg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gahqxkpob.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gfsjmmyqp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/glgqvvptx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/guldbnagr.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gtwiiohdz.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gjctizkyv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gibitcqdd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gwtlicckx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gwmwnotpb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gpbxfofxp.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gnfbamrfi.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gtuhdkujg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gaygarbxt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gsnwhtpqb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnzekejkm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gdjuqfids.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gnfqefchp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gghgieivy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gqjkuqlry.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gynxsbvhd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/giolpslne.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gaxlgwbec.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gernljqsx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/geiexfirv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gaxbbqmey.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gakdxvdhl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gbqtjzvsu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/ghoeanobn.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gdlluseen.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gzhethtbh.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gwyxbcrim.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gehmxatpj.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzjmjmqsk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gowoacmkk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gulhkuwdw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gyqodqhuy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gikbbqqaa.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/glbrjszxc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/ggevtmrra.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/guxgaxuwz.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/glmykddjp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gccjshioc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gqpwkdiho.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/giyikrkrc.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gndthvqlk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/goxstktcz.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/ggplxsjxf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gjxsnyzlw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gqurgqskq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gweelkxqv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gjmcbbtbc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gbcbcymwu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gvvvxkbsw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gdudqtaic.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gtgfaaleo.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/ggepwlisj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gnpmzyvdf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gfbkmgkln.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gwyscaoti.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/grzqexsix.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gduarlglg.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gwnvxbojm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gqostatyd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxkxzyvoy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaxkgcayo.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gdwhubtjg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gujqbgdbr.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/giahmwqix.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gkvuerzrp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gajwiujav.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gejnxhjod.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gxbtqwqfi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gbzxbaxrt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/guqqztdmz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/grkzrhmdc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gmynkvdbg.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gndtrfdvr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gnckacaeu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gzryziepb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gpfvqsprq.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/givtgznmv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gzsfuhkin.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gezwtogoh.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/ghnpxyzee.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpsyxieob.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gwziqacwy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxszjyqju.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gatcgfcqq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gpvzxhkcf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/glmmmmmtr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gtyzivael.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gylbbxfyq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/grgretoda.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gpbogrhbc.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/guwlvjhkd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gboxvfivx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gbgaotxry.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gpkdozoxi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxclzoz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gtxlrrscw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gfisbyelu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gtxazvawz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gprptkepj.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/glvowrvig.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/grbezjgdy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/grgcmjebh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gdgdpvinx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gdxildkzg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gzycsadfp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gfvuzsohw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gvftszifl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gyfbuxnky.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gydupqbeh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gxknebkzt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gcshqlgot.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gyzvhubgs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/ghwewowfn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gtdmrpdfw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gsdglmcxy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gcrovizwv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gydqbdzmt.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/ggsefodxw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gtfowbyki.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/ggxucoaxp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gkxtdzvqr.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gkxhkjbns.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gikhxtamj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gwvitacll.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/ggryqgpcf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gegtweyty.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gbrzqrqlx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gtsnetqom.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gihotvxew.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gxhxvwtyh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gjlebcjdb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gyotjvlfq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/goonxihgg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gjccyjlkc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gtufowcug.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxyzsniuv.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/glvzcamyt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfdtybgsz.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gupxghmvy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gxxaliaza.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gytkdsjfo.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gmzjzosmh.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gssunpvcy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gfcukhghx.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gvmtbcfvb.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gyycuuqlm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gslmatypx.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gtxqevwxx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gmaffmacg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gqxszacxb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gtppphrya.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gyhwijrje.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gbdkonnqh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gxwxrdyku.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gaxtcvoyg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gyswhlyew.sHtML


<!-- 参考信息 -->