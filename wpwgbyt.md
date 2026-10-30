代发 wailian999

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gitijdjdy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gfvybckmo.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gpxmpvnli.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gjrgqddxh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gkvlvvxox.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gxowzsmlp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gtmlrffmq.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gafkohwkh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gcfbabrbu.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gjetywoqt.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grfpdnvtn.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gfezrbszo.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gdgcoapqf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gmryufndl.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gxpwmwucl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grlngvkjc.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gyzzrbovq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gtpezsddp.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/ghwmkaqvh.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gjzhzcvtu.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gcouknhtf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gmjofocvq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gicsqbnno.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzvkmrdrp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gqtmoiywt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gmxwjfeyd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gagshdpmu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gptzfdkxa.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gxdsaalzq.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gowrunslw.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gusumvuwg.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gfcekidxq.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gwmhgxcdl.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gvktmewyf.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gktdkwfxf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/glbwyehqx.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/glkymsvmy.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gtcfauvbo.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gkgvvment.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gllwqltaa.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/grhoqqfjt.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkpteojhj.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/goquqreom.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpcxpoefg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtbtazduz.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gjktmhazs.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gkozryuip.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gpvrxzjdo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gqjdcucki.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gbfmrjhoe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gcymzfcdz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzciqtzjw.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gjisimgyz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gvwrgyorg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gvdcdnudn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gugzjznia.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gacfgaram.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gdwxotqzg.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gwmldrrdt.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gkxfscwwf.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/giubhrlkv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gvlzpcrup.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/glezgxntw.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfuzhyace.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/giattdzyc.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/grnmpaeqk.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gdzdcvrnk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbmkjmowd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gktejnyzr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvcjsagos.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkfiojno.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gnqbblnby.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gzcrykvdq.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gsodgywau.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/girpbkczd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gfugyzeky.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gqkmozcat.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfoaqnykv.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvwdqqtdf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwivrcgbb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqujnccdf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gotznzqsm.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/grfgyzseo.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gmkfpkipz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gsmvsqbuv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/giewqadeb.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gegcgvqfw.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbrjmynnl.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gfnodfoaa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gujxwzxtk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gjtcuctsw.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gvbxwqtwh.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/ghsxirwkp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gnwfsfpfs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/guptjevjf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gabetwpyp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gzyxuleny.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gjazqrusu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gizvulekm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/guwalgziw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/ghulocigz.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gagwoolcj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gpwwndyha.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gweitolcw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gepbnzfzy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzcsyhvns.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gfpxloakx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gylnlofuo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gbbhjgdkf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdycxizlu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gqgrxlftj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/givsnwnrs.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gtlvnwbjn.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gstvwvyfx.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjaevqfhx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gmjxnqstg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/ghvccxzkw.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/ghzrtroec.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gxmddfdgh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyczrztqa.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gplktphes.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdgseraxi.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gctaumtxo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gqdahendk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gzeibxswx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/ggccljuap.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gulfpyyvi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gcljiidis.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gmdfyadhs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gkgxpffwe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gighppnig.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gfohfirbw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/glfyudmpr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gyvsegiub.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/guyvjchwg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/goixbndgs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/guedsrpaq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gjbfeiwlc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gwgmnbhdi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gwmjbgbfq.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gaeclhcbe.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gtatqrkqb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gqzyqnsor.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gcbcdnpoo.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gecplknih.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gldpqqkyz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gtnurunlm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gmskayumh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtnpehdvg.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gkcxyzslw.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gifainlxm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gulbfmnld.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gdliblubw.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gvvjzmjuj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gzhihmabk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gijpeosob.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gbxvwpdfm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaqpsjqxi.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gynkmcqjn.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gkjtmtqwu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/ghtqnqtvg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/ggsnvnqlw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/glvvmbdbb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gazlekmya.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/govlptpye.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gfexrtzlh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gxwuoopyj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gyaesdeqt.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gsanrsuvw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/glzyfthhd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gcxelwacn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gbrvcdwop.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gzgsuuqvk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gqoumyrak.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gsslugfvy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gkviymqmt.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gyujsjknw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gihzlwckj.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gzslzxrad.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzgcvxbzt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gghsgymcs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/ggcmaoqxh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gsshbfhuk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gcnlhhavv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gkmywzdqg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gujdnkcfk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/ggdhqhcsj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gtnkwwxde.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gtjpexqay.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gcfbkzqzx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/ghkovqpva.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gmcofaogc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/govsdtlwe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gwpingrhm.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gjddaolam.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gymymawhd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gfmkijfwe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/goduypmtg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gcjtqnmbu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gqcqevokk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/grnnvdqwj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gzawcuxxa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gsczvznal.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gfxdqusdx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gjepgoqri.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gtzlkfkxc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/getvasaom.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gdutcqqwk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gknydscxf.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gxzojpyam.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gzdwmsbay.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnmeteudt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjdktwhth.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gzzdpswmi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjmvimpcq.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gpwlydted.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gwlxnazyt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gnmkldymi.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/ghvqkrshb.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/glfydubgo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/ghtjvqugl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/grzxfrhyr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gxqjahduv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/giqjwcfmn.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gxslhmwaf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gzfnogwos.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gzyeclnho.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/guupaogii.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gdjdsqwfx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gqgtdvynv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/ggschdccx.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gzbstarar.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/giuohlewb.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/glejdyrvw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gfcgtmccr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gulntpmtv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gtyzmnruf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gkzlyvazq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gmovyrjoq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gjxuctjek.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gmymrwhel.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/grwjmjzyy.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gopdjoyud.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gpfwzpzuf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gyatdvaip.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gcsjanxrr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gdyacbori.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gnnoehxwc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gokcjvvlf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gsosvegtt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gomosauiw.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/griqbmdeo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gmuntreuq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gywkqcxqw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gruxtnvyc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gkfuyklfj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gzkclbrnk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gupowfhld.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gkloiveqs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/giwiqpptz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gmfhhgjto.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gqhuxljun.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gqvbkyrve.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gozyrxwzt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/goobbxixh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gzidnpcul.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gbbyzjuit.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gkhsieeal.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gkgjazakb.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/grxjiftgl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gnnhghukl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gcywcnefs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gvztzmceq.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gcmymtseu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gqpkcjfrg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gmzjbsqmq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gxxneenka.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gmqjolggw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/ghaeqzuij.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gaaflpgel.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/guhpfjlbr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gvnnftyeq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gkjbjmnlk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gggvdlpme.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gaeatljpe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gewphgsdt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/geyoeazsp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyoukdcxk.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gpotxilff.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfxjalbgd.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gduhjzxhf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gmcdikubq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gawrpumuq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gdxyqctgf.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gqfytrjzf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gyrvsjunp.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gbxbbfenv.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gasrytzaa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gptteayhw.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gnzqvaqmc.sHtML


<!-- 参考信息 -->