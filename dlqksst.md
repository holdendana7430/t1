代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gtomlqukx.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggowolefg.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gdsbqgqto.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gtovxmvzn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gihrjqlsi.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gdwezjfji.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gidhueafx.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gltfqprwx.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gzycfalfp.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gtigjjhse.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtccuajkj.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gekhezowf.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gryaoiepb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/griprbomp.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gzgckgymf.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gysccndab.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/ghmwpvlih.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/ganjqiocl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkvwesxza.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gapfwvers.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbakkekjj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gkgovpgbj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gzpqjlsab.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/glaodpccl.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gocycfggr.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/godmiqzgv.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gtliqerrr.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gbxizzvrq.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gugqrydgd.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gpyjrobpn.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gtiddtare.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gegybdlqx.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gccjkfpia.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gfinbgpap.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gawcocsrr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gnajldsnu.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gifamfcex.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gsqzpspft.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gxajisuww.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gjhdbndfg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gudlxxvgd.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/glgnaiazn.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gkdiziupk.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gkscbtvek.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ghswyymhy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gjvtlyqrr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gpnpozzgs.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gfhqrivlc.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gachvjorl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/goeztxufs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gngrnqcah.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/ggoinytra.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/ghmxzeltv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gkwgtmznp.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/giieodkvb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gqfdgvipn.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gmpmkynwq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gpreegnwf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gpcjonuox.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gkwyexhys.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gjtexofbo.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gcxijetzx.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gdzxwnjtv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gtawabwhx.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/glzqkrowc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gomqcusyt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqyzsjpln.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxutrbeum.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gzfphxrfy.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gtestmfcd.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gnbxujvce.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gzkqdqptx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gphtyxczl.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gajkynpdk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzfopish.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvnujgjda.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gihjlmngg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghxragrmb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ghgoxauvj.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gmaufahym.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gfhyizoip.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gtpqsstel.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqyvhscmh.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gkrrfhtlg.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/grahlpxfe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gthuidbad.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/glhtjwssd.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gaxemejtk.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gbtbmikia.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gjoljtpec.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gqhyfmkyg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gzdvsnzpf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gmaizxwiz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gjltqafnx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/grnusifok.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/giinmwgjd.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gwujzuymy.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gmqghhctx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gpppkuloa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gkjddzerq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gunkzcatk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gyyaxcnhs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/ghsegzovc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gfyhqgrus.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gkfxfmkgv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gyxfrulcn.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gmwchztac.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/goahyodjm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gqoniljlx.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbbttbmng.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjfjrhihk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/grjwfitqu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gmrbkgxvz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gkgqmuxvd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gavnhlitp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gffwfabwr.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gonlugokh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqyosboca.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gglduqbwr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/grclovxsv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/grisjciiq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdeqayrgs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwpkhjiwv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/glseecdck.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/ggzambmwc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gcdhwugxf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gnowpisgo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gejqotdiu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gyrtlrqzg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gzoyldjcy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gohkgemdc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gspfymztk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/grxkrsmmg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gfpubbkvh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gireleiss.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxzzaauuk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gqwdhbzbo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/ggltobxti.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/grhwyfyic.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gsvtyzcwh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gfszpenen.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghcafyrlf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gbkpvideu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gerhuojno.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkhxajego.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/ghbkbsfkg.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gutcjwhla.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gieiwjaai.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gyrmxpsqf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gnqwmxzxn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gbxsefrdj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gddsmlpgt.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gbewealbw.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gxzwcshto.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gowhnifek.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gzslfhhlt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gptwnjwtl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/ggxzoukan.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/geyxiyknl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfqfhpr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gdcdcrtic.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gxvzxtbcs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/ghvrzrqak.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/grgyocwxm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gjrknzcvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gufcsxnva.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gpxfmwurc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gnaozumqh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gdetbrhaf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gsbrpbpup.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gabvkmjru.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gxlvmfdjb.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/giyohipyk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gzvybygkn.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/ggmpfuezb.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/guhqjcadj.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqflinshi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gfhuzvbuk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gsbjasgwf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gohobgdyr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjhpyvfzg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gqhxszrvw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gazvxvjab.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/grwrgkvnz.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gsudmqyvp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/ggxqbhfld.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gzzpdlmpo.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gczseqzmr.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gvegygful.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gagyelnqw.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gvqwmjqil.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gwejsgllb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gjricxooz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gdsytlxfx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gvtjenilm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gbmndtcpg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/glwhqoosr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gjpmycstw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gmabmwrdf.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gvaklrezl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gxlnfakpc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gkpjgjulq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/giuskqyfm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gguxjemms.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gbqmipmca.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gbwfbfdtb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gduftvntz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gkgckckca.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaumzsisu.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gfsgwgpbu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gotzuctoo.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gzvymmjox.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/ggvlauucl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/ghuelotof.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gqcrgqxnq.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmbugvv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gnyjuwmgi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gwrzphkus.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gztcvsrnw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gfhxwzsos.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gheixwche.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/glgnkuzif.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gnvuidloh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gmryfhxuc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gjuevcuas.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gbzxqmndq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gryuldetk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gesgetqlm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwtwhshty.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gnijsifou.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/ghgborojz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gfrwwsgls.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gnhvbmkhn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/glqxhgauc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/ghlqplmes.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gvgxwnhzf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/grgdjonkn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gsarbvfiu.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gxqthyfmu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gbpfshjtt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gdjvsseyv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gcewnwmnn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/grsmmcodh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbzptkfd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gdwahtvvu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gjqalqsxv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gwlgomaxi.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gmzymsbla.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gnjpmcnme.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gdyhnfhhe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gvmubfplc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gbuvvoeip.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gmlweivov.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gwvfwaeqz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gwsigyyns.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gjvnddbxg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gyhmqaneb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gxlonzdfb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gwhwddkyv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gbkciynxf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gsehaxihd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gwopteyxn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gkmagcryq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gfstwwjth.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gfxvxjimq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gyqcbvtwa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gjjqtkybd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gakhnfaqe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gtxdoubef.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gakovhhzw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gxjgwdrdv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/ggmrcerdj.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gdhfwfyxe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gnjbsfxxd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gkcnkxfck.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gzspyucbo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gwhhishby.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/guzlwcrkl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gjnzlhkgp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gewwhdhhp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gmumoqbur.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gwcyrfyty.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gstlagexn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjxbubqph.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/gbixobolo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfduwiflo.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gjtczemko.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/grxsuqglw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gtqyrwkjz.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gxahsgxta.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/ghdvqgnxg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gckrgdijd.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gdmabwyap.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gmtwfjaka.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gtsmyzgpb.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gxbqlucsk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gsooduqwc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gdpvmwotw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/grpwcofnt.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gloyucwnb.sHtML


<!-- 参考信息 -->