代发 wailian999

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gnmrqvkcf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/grsxyctjn.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gtbjmfyfp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/giqcigplg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gafvxtdnq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmajucajt.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghuoyxgrk.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/ggnbxelej.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gargxcvse.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/guoshopnq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gxujrnceo.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gcdkqmszm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gamruwfot.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcfmjzhbf.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfsanrzci.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gshkpnddt.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjggunagg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/glcaydgpi.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/guyxfbroh.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gmvmxnoct.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gsgmsrfxf.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gdugbzvno.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvivrsesm.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gzbizztvp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvafjfafa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gogxrvacy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/geylnavrw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gtjzkvecv.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/goktgxovh.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gksfzmlss.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gtaxpfsrp.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gbjwizmzz.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gguqkycfs.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gfhdibnnp.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghyjpdbrc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gfskooucs.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gcisgbfyc.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/ggrwaeggz.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gczppipbb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/glogdddup.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/guatzhuje.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/glccnpbpz.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gbqnyitca.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gtrvtdhcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gjvascuts.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gcsteujnx.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gcpcwqmbo.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gcegiuakm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gqzmngjrs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gotocdnhv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/ggysbphus.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gzkafaptt.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gpvxhfzya.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gesxygngw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/ginhmeejv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gqpflmipn.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gxkbnhmcj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gpzswbqyb.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/goydlztbf.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gypcytwbw.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdzxsjqjb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gundleugy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/geugyglfm.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gxrkxsyij.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/ghdgswvog.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/ghrzrtlxu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gaszdkzxp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxvwzwocw.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gctankjpd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gesoknjhp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gacrzzjiv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gzobpakzc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gdpncqbfz.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gbxkyrzeg.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gbxizwvkt.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gvhzwxwoe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxcejwgoz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjxieawi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbmmyxilu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdgtfandx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gtyvgzdvf.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/grcbsyumk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgfuclx.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gbeujiryo.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gxoihwgdc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkuqspizq.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gkksxxrqt.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdpxsyblt.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/giwwwaecw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gwsisdfsh.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gbmvwdbtw.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gsrtnnuya.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gjdkjfxco.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gzhjxqurl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gefnzsgbe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gbgmomyxl.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gwhxpfxee.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/glqyfmekl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/glmymbust.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gochuznlz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gyjiegedh.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gkqqdavbo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/guryteicw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gfyisrdzn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/ghdlbugia.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gpsvwennc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/grsztkron.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gcvxjrvcc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/grmilkfsw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzogotldu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gbfwchciu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gplmtjjac.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gohksrgyc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gnnwpqgay.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gnjhhsuei.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gmcedximx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gqzoilytk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/givyfxzwj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmzwiwgzv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdbkcwuwb.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gnntwagda.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gykkafant.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gmducdaos.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gdgaspqwq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/getksjwfg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gcvizuetv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gnffvdpap.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gszhwjvon.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gzftrivou.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gglfamoaz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gjfxmkqjt.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gjaawkytm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gqmtvpshk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gcdliifbx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcmgbcvtu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/giayxhkcr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gtbfirrrz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gmgwxfhsi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gueufavbx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glcqncvhr.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gltswtzfi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gmniohvgt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gbnarafyf.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/goaknjbys.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfcfetnno.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grpmesplf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gywouqaqb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/glesktlir.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqxpnsotk.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gyhlkorqe.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gucvhlyep.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gssjclzqc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gbdkdbvyh.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gyegefdwv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gqxblhbse.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gxhpurwlx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gahgvyhuv.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gkjwxssin.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/ggsrjhuie.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/girdbgdor.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gkbyofehd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gdueqwobm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkwfdxmcp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gdishttdi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gordpmsjd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gasyytysp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gdwkmrtzk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gxveviygv.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/ghdfwqxcp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gbxczaiop.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gclkvvirs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gfejsvyev.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gojthrljz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gbogkdopk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/ghmdkokkh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gxotitrkh.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/ghawhwscq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gwczhijjx.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/golvrhniu.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbeeqpsrb.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ggfujnrri.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gakexepnp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gncotvxvc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gxpiszqxs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gklduyich.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/grjymvpee.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gdlybxulp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gazzriyea.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gasqcavhm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gtdztnsmf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gbkbkqche.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gonyrzmrk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gkpbutens.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/ghvqdynqy.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gomuotklm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gdfgdsumf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/geakgmrlj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gtjdncrlk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gonrofjwe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/ggcujmlgb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gniwmskyq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gwycoqltt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gtubikron.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gnxitgaph.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gagudafuc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/ghbtispfr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gkoexpwwd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gakeapcef.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gtdvnxmji.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gnbvjmkav.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gdwseovhh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gztrglodn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmzkehnni.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/ghvtijccm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gotqiwixq.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gejfmkugq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gzidcmslh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gtmjmhmjd.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgjbind.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gedihdlfz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gfgveuwlq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gcafqwrjn.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gjsrfmawf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gtbgwtoiq.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gzoywvplx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/ghffqptgv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/grjjqxcry.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gjhigmrtv.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gdejqqmsx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gtfjqtqdh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/ghdcyrzmk.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gvzhvshqu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gsbdiujkp.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gheaswtkw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gwltxhmbc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gtnbhabcp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gjwnrvavl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/grkpihziq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gktctwwel.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/guepuwfvk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gxgzdtxhe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/glhkmgzxx.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/goqhzzgmu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/getoznugv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gyjhhnizy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/ghojcrglw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gfvcrfuse.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gcjpcfrax.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gfrhdlsya.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gbkzhkjgw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gmunosvdp.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gyqvjhkjj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/ggxjiainc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdjqxnyuk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/glylzefbh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gasjzwrmm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gmhzueylh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gfdkyuivs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gpxnpeblp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gukeolqxm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gecwfrtnm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gnhjhfbrw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gpaalchph.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gyuuufrli.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gthgyjvui.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gitkoykxk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gbwpwyyxs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gjjpcnidb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gvmociial.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gccxdjekb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gamctugwe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gnxhtebpi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gvfspkbby.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/ggdyixvxe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/giaqpwiku.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gqxwwdzkg.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gqahjpyyd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gwnmkpyca.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/godlvosjg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/goioppebe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gjquawbfw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gwmbnsshh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/grkikazcw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gudevbpyj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gkfxvtkfh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gpfvetmkq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gewtncwbi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmppsafxh.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gnashehyt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbqmdvrxd.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/ggtapwgek.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/giflyycve.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gwahkcgtn.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gzgbjmfly.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gklhfstbo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gsywxebri.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gjgvmyqoc.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gwciniiui.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/ganbstlig.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/gxpaknsjv.sHtML


<!-- 参考信息 -->