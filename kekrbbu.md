代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gleeijxrp.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/grypgdear.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/giggzrdwg.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gerrhpssm.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gwfqkoqcd.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gicmidvwt.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gkvlxyomn.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmvhdgwrt.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkysqwpan.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gxhvyvgyx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gwazxpziv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/ghvimfuqm.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/glypoghvt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/guhhcblyk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkdpqduzq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggbffzxtm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gptnrvegl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gkooujbjo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gxcopekcs.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gaggzetbl.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gccvgcqpl.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gnfgznrgk.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gqlblqewx.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/grnqoxgkg.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxdwyavwa.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gfndssqds.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gezzfpgpa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gckxztuil.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gsvgjrwme.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gwfzjxeyf.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gehtkkcrw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gnwkkwmsp.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gyavaavja.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/grlxhjjnu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gewduxiux.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmlrugazj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/ggzmbvrgj.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gtlrvvaid.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gamlkxxrg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gcucfmpml.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/ghogquagz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gpfyvtlbe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gztqtdgou.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gsiljzwjf.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gkrkptqhh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gndugtxkk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbgsvncyq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gcyjyuiyr.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gascjtsdr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gxdkhcgiu.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gvenwihkc.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gxgqkhlin.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gkbtrnlqw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gmevgluvj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gourbvcjt.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gqwielzwr.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gtklnwuqv.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/ghcrolzvz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ghgfqawhk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/grirmyghn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gscsavvkv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gjhqhmrpx.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsdjzynyc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gggrwwkyv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gxxghelle.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gjflmbbpy.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gozcrqrjs.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqaxmohuw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/giwdoujfl.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/goeezttfa.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdszxfnws.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gjctiyyga.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gzsjygurk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gpmlaykkn.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gqaqwjzhv.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gvbolseko.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gtsuozwhd.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqjqvozni.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/goetnombs.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gyjazlofk.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gisvkfhcz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gsppozujf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/ghirqygmz.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/guyplxyhg.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gztsritnb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/grhmghoiz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gingwyoue.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gnftdinpw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gezszvirg.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gtclxxfqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gxlvszhya.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gptlfqdaa.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gotxbaqux.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gwybbqdbc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gsqyswgjc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/grnduorbp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gtiuupcnc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtgitzwca.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gxilaodpf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gkijmfvzh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gbnjiwsrj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfukkfhvv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gmmqirxpm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/guncqnuvc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gtecrhetm.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/goypptzdq.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gdwmafabz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gcnzvcmzi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gomfidxad.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/girdecksy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gnyjwmnfe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gynuourpd.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gzavzckfs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsbmfpypz.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gbrtugyhl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gjmotgijf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/glmakebyw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gczmshgzf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gwavgicfd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/ggvsvrhog.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gwqwwwkbw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gsqgsotch.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/garxxhphw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gomdwuvgg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gpsnablgp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmotvcnxi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gdgcbnimu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gtxbdfvge.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gznctreye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/ghrlmrymf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gudxnzomu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gblmnjcym.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gltpausli.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gwmeghbkn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmraovrru.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/geuthgrur.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gupcyohwg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxuvjpqtu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/grpanxfxg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/ggevattgn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gugtvpsuq.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gdxotojwi.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gmlwgqdwv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gtfvgffcf.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gdfeazzvf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gqttljecu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gmagbdwli.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gwywojedx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gqerzavuf.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gneuxqxkv.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gmccgield.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gqxzlgmsx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/ggfflzhym.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gsmvgnovz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gxgnevcei.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gzanhyrux.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gizpoxjhy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gqundmiqo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gxybkkord.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gfjrempxb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gpwlzhqsa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gyoogbuik.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gybvvendu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/ghrcpnree.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gtecrmjep.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gbaeyyuhy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gzeiqgurg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/glbsosklb.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gesivzpxi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gzdogvwft.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gjjnzials.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/guhedoefl.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gtqnkugpy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gjqrfovgr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gfnjstswq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gxialegpa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/giwhorpzx.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/ghuseschz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gndnwhlrr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gxlvguxzx.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gufrjlvqw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gvrovfvdl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/ggcvqvznz.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gdxpomhsy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gjhkafvfa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gzbmozutg.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gswjjvzpb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gjuqbcxne.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gbofjfzoy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gdnozcdzf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgtrykok.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/glsymqszf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gtblflzup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gkmyumiwu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gvjwlqbxx.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gmcasqvjg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gkyqxfkfb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gnkxzfasl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/ghibdyobv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gnzbkbosl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gepdbjait.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/govnwulpw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gqwjiaipa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpardjurv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gictesexe.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gsoeoxetf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmxitwyzc.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/ggosnibai.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gtbkueadt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gcvipzkjc.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gciiyxygs.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gnhxrxcsm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gesiqwygp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/goinueibg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gbzzgamdg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gbxekezbf.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/ggnxxyloz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gdimlqtuy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/ggckcenla.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gztsftxfr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gvignykra.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/goyugcivv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gkqqydlvo.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gafefvnvz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/glkqfwnwz.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gxuplslcx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjvntiht.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gbomztfed.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gaglezvvn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gkewshpmi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gjhxpobwv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gkfzbxhwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gnmidmvce.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gzspwudug.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/ginhpteuz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/glmcxkngr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gunaxsigg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/ggrfkzzcm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gfszwmogl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/guwjllhnq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gywzbhecy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gocqppxxp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gfybnufit.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gjleymnao.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gmgkkvgep.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/grkyqjusz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gvomuowsb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gzeqvjfcg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gwvmumlos.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gxumokwov.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gxfqipyhr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gnnxiucmd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/ggyeblaqs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gtzrnrbgp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gptyrwovn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/ghziehgph.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gylzfuqdu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/grshsjpxy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gplibegxs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/ghgprwmgk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gwxjirziq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnrllgf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/ggvqefude.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gktvqhsxo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gfzuqsfhn.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gyowlgfef.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/geqzyiyfu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gmlruzwxn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gkwdiyegg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/glskdcuxs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gymzwbxtw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gdtcdoqdj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gjwpweadk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gqdodxopt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gqtxwztaj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gyvrsqsgh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gucmnodyq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuebwwph.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gbenhbdhd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gducdctte.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gwxambofn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glqrrdrwm.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gguacwxnm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gzjjirqxe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gjkhtybuc.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gphuwonjj.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gwaeizoud.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gntbwpkom.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/guwugmgyl.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gyqpsjgqy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gewrjgcsv.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/ghbgeqjtn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gbriyszke.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gzuayrsvu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gurkqyytu.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/grwhajecr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/grlxesnfn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gygcnxlgr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gexafiqke.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gcbyhhjhz.sHtML


<!-- 参考信息 -->