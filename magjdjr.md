代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcpcveyvb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gvkiuztha.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gdquwshjv.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gvcchylqq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/glkvivtpk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gwxbmldin.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gooojucjc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjffglsgl.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjumrpsos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gntaotuwm.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gabplqhog.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gydapfneo.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gecmbaalq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gpqndthfc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmlfmxaxg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxpeibgkn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/guztupudk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gejklqhmd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gliuocftr.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/ghqfmkvke.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gmejuzfhi.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gjipeubsa.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gcaznhifm.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gpnfbrnro.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gsngjzeta.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gtqhbjkbv.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gexmsckhz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gyvzdjils.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/ghfyxncpc.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gulyaavyz.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gbkdsgplj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gqknkuicq.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gkyoygtyd.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwjfszoau.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gwbyhbdwa.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gfapuguen.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gkwwygdiz.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gkqtuvlpp.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gcxoyolsv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gqiuvnqoa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gcwsnsfmr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gdrjgdwub.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/givcijzdj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gdutvjzip.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gpwoscxrc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gcajhnuzg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gqrcbfhhl.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gqkozzkjx.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gujqdncqx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gqhlibeyu.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gglfqcfqb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gpnpxysik.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjpbmjtzt.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gnetuxvyb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gqxatfpvk.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/grjybjrhw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gbpaxaxva.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/giskejzjz.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gzwlghuwb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gjmaoyyjk.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gcqhfvnsn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gautqmbuv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbkomogbl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gitzktvhe.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gzrxwihgz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gribzpkqe.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gqzftjbgj.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ggolrcucx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnpqflhnv.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvxkdcwxu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gyajmrhwk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gzrdqcoru.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gealncswl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gdwbiskhm.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gweorrhfp.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gcccvweuu.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gecbsllhc.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gqpysxuxz.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gdupbrswx.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbilgiyok.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gbxkbtwcy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gnfjtgtsg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gnchtqopk.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/glbglcbud.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/giwhgfngs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gjxuvcaia.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gqdbmizto.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gclioflhy.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/glytpddgg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gdaazizya.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gcuknvufu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gseytnswf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gwjliuydq.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/grhkedwly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gntpybmjh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gormsyxvk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkpaftm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gotsgbwfv.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/grimqpxoh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gfbahdxoh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gsicjuuem.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gqpecmxzb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gcodacuua.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gebrzwcpl.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gwxdibned.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gywuuezqz.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ghakbxtrl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gfrsqhaca.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gwubhiozs.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gspeqitlg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gwatipnhx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gomdukmxe.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gaanrdbqj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxvhshtqk.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/guhhyqmjg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gcwzfvtbr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gmvrceflo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gndptnfrx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/grtgftjga.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gmjixiqjc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gzxpsghvh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/ggkwtbpqa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gvjlpzdmk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gouqefqst.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gciwvbgjg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glqmaklyd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gqbszrcns.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjzgmxfkg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gpixhxbgb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gghypkcgb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gpbywzcwc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gciiefoso.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gbvkhvuhp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gkcdhseyb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gjatnxfnz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggaloflou.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwrsyrffq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gigcvaadb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gjwxfwrps.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gnjcdnjpc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdrrppjis.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gtqvepigv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gshfiuncf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gaaaaiilc.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpstzvemx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gislevsls.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/guwzdlbdy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gtnkgofng.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gwtbsajbm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gsfrizgyq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcmeirckd.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/govkkvqkv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gftfcwgln.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkqiqnmzk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gqkztizfu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gurgmdfpg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gyxkmsehu.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/giepdxwbx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuglyzb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gutzhtdrp.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gugduhvio.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gvwmrgsqw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gimkbbeui.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gyskqlgrl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gbfgbdhua.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/ggvtljksw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gkxeejqjh.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gzjfkyyfp.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gqngwrwoa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gzqvzccpa.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/glyvuanhw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gzbiltxnb.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzqbbrrnb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gpkgnzcqr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gsinafqxg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gthqvjrdj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grrrqgfhm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gdpaceybw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/giryficqi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gqwcemoxa.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gncitysgt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gkcnlqylg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/guorlseqk.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/glueejvkl.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/ghsfahdhn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gwgovrxsp.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gksiylkeq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gxlgdvels.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gsybpvicl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gjkatqkwv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gqnakrceh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gwphvzbdt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gbqugipzm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gyscnngtj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gtnscyjhl.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gajsvuklz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gxaedmtgh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gzbpoewsx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gkobsewnm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/grtshocka.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gpocwacwg.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gcyzlzavd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gdvbjiigs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvorixbyy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqllzlcxs.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gvpoyblvu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjdmefjen.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gnqsbeugd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gpylfyrik.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/grigawfvj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkdokwtuc.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gywqgvcqa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gllqwkigw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxbqiyzcs.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/glpmstyod.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gjaaxtwwt.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gcemynbbj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gyoludeln.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gyoobjino.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/ghaceriiu.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gtqhkhxcw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gyixferte.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gzsgyytld.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/goidhozkv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gspnemaad.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gizxxnyts.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gnxeizbfe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gxhbaucuw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/ggrysrzid.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gajddasgi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gcrqofeiu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gsrylczer.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/glbglcbrh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gknoqsake.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gnpjlqipt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gdsodynrf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/golnuydfs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gecyhxexy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gdxjvhatu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gqjrdygbl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gghhaxryz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gyveewwcr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gkhhwkgsf.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/ggggnissj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gxyevrycd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqahjtrar.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gimbgjwdc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gggzxsrbv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/geqcfmujn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gaysbqvcd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gtfuoklko.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gigocdjjk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gsbvbwhwc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/ghmxxqsvw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/ggijdezss.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/guvxmmphb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gldnapvpj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/giwcgycqy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/goeoplhtg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/glubrtspx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gbzoeveer.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gniifjpgo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gfacjtnpx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/glmsegxeo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gqzuyuwtg.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/goobzwfev.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gqkkkpvwu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gpwzdbcdb.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gyszijwkx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/ghpjxaztr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gshkxersf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/ghtjpjllr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gnzmimwqw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gqykdmnyw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gkvtmgjnt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gzuouhcdl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gvabjizuh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/grawedira.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gtrzsuavv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzjweflze.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gakajpbja.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnltavspk.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gysirxabv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gqeiovozg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gnilocoti.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gigkwzkqq.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gxrpobvja.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gfhbuznda.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/goyedudjy.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gwpewucym.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gzwsfrrqx.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gvzoyhmky.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gqinniavz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gtrvzqsku.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gnumbkxow.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gtssojkaz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gwyrloenr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/govoehjdd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gmhadgroz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gtodvibwv.sHtML


<!-- 参考信息 -->