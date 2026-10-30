代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgecxuel.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/glzwrqbpa.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gljieuqyf.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gxzzocger.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gghmqijyn.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/grpjsqrvp.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggjohoahy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkihktvsw.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gvsqclxkw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gdzqbfwyu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gzzmlaitf.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/geclzlyfl.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gwwrbbiil.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gwlulinit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gobgzlatu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/grovrzcqw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqchayezd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gqinienwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gyhqecfze.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/guvvhcose.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gswbxkkef.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gezbdxcuu.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gveluvrmx.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gofikidpg.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwodzbzhv.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gkiuoacwi.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/geqzbwdjf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gvdlffynx.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/ggwhjmxqv.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gzvxyavln.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzabrdu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gzuboaanz.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gglhxqgle.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gqqdapnza.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gfgpmfpoe.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gnwgyhpdo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/glmkmhfxe.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gdqpppbul.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gdurckvxe.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gjbqtebcd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gbaalsmoo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gyvjwzybx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gdvpysjos.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gwqydmxeb.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfseqpiti.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gjqgrlamy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gqtotcwxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gbunwwcow.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gmwhawuho.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gqbazgzan.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gaqulcvpw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gtjiefijm.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvujhbnpt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gkmavusfm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gmscqqfim.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gbishrlay.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gepzzayjg.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gkdwwbpqj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gktqovdgk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/giolgfvnx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrlvhlhb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gimeuzbyp.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gruoovsli.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyqvchkd.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gzlvyjmfi.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gusppforp.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtsmnsazi.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gkvyolger.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjeeqdmer.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gssqacvzr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtquoujzq.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtacmmjbk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxhhejpy.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gsrfzldfd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/garstuxie.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/ggurwgqtc.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gjivdwaqh.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gxsczchfb.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsiwsthlf.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmezcsbet.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gklrujceb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gkkgjwzhp.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gjvayblbe.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gpsnucwsg.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/guenukcrj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gtpczcqxw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gpswvverv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/glnknznwa.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gguclbesi.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gbxhtjfel.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gngtnkymz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gpxmptjfu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gaaknddmx.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gcqgylxwe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/glgcsjyfs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gmqxuhant.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gojapecty.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjlllvitr.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/guroueyim.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gvdeetkzo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gzrlpwziu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxbtzantw.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gpejksayv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gxdcwkmic.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/ghuytdvlm.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gkkgtlfon.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gdwpdgpim.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gxxlpskmt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/ggaudpdtt.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/glgexzoxq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gvodskmxg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gggtxgpkh.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gzteiyiap.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gplizhbeh.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gxxzcyxxr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gipgzfybz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gxugcjiio.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gvmyvchlq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gxwkakdyp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gzwmvtwvr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gjnyjqhdv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gtfopgfxx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/glnnietku.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gtcsmobul.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gsvxgexxh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsydkxkhh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvpjpcrcy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwtcampqy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/getyyfavl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/ggxcvjtwg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gxcleuhet.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbthvjjcc.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gbeqioyyo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/ggakwqdgw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxokrgrnc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gikxhwvev.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ghumgtjyj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gagoxwnrw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gweaoqyay.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gybfqyphv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvmqqvusr.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gnghsyhlk.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gywzbfdft.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gwmpufejd.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gxbggefxl.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gvjkuqbvl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/glvsarrug.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gbslqojzu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gcamticaa.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gzqpwxqex.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gzcnzvhwi.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gmgwnleaj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gluuyzpmv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gtvaeskuq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcggyibrc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggxcplowa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gdozcjidf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/goqnurhan.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqvlikxra.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gvignyscs.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gdhcchcey.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gaiitrpgc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gotmurobu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gjvycdxxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gtmkdkfdt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gsqcvutmy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gaaliyfqw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gdbwxfbgr.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/guksibarl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gqnmueebt.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/geqrhbymb.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gkuapmthe.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gmhyorabs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gzmyxqhjk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/ggllxnlow.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gyvaetckk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/grbzhxayf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gkbmtnatx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gsrkwtvby.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gfvzrjoxb.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/grgktgtey.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gkompmwza.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gfnkmzimn.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gihuftlqe.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gphznufxv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gatxvxgyg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gajmdhaos.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gibnjblxd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gbuvolxmb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gkrjgsvjz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gpncoclgz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/ghdbwfrge.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gdohvayyh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gskqntczo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gshlvcusq.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gqgxsjott.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gqtqtkhiz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gxqqjdlce.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/ggsgrgvmb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/geudjwgok.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/givfndvtc.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gcozewsqf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/ghndhywam.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdofcbkkh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gderiqovi.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gibyekuzv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkmghufjq.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gevqplerc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/ggecxthpr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gavoxufxx.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gusyikqaq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gpybkuptb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gvbexzjws.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gscfmjcal.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gwghsodef.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gbbqmycpx.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gugxocroj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gjgsnifxg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/grliffndo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/glceydreu.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gtvarxzzm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gxrtedvdk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/golbgvmxi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/ggiziqzyi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtjbthjwo.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gklyxpuvc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gwvpqdhao.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gfrojubqp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/ggeakvhiu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gfddguizy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/ggxiwovcm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gjetadqgm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gpzxyvnzj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gwtvgqefy.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/ghlelaskt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gkuovdkce.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/grywwxxhq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gfjcolcdt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gzhhxzlpp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gwxzrnlbb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gydkqljvx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnrtthtmo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gpckfuuew.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gknmlfqba.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gjndefars.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdotmzisu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gbhhnssja.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gqirsuhdg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gfwinbjpq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gvpecsmch.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gncsztgcy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/givpysqok.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gfhaeavqs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/ggymqvndt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gjpyzniyz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/golhefops.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gfkdveuuf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gliqmerow.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gdnahnuir.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gvawnjhah.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gzuzyqlbh.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gfpbwwwco.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gwvnllesd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gpiulaiqj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gwivdhxok.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gbmsncisc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gnzewaxtc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gzyaqhbrd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gngymnjea.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gwzlojvvd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gphimqima.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gaqhficop.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gcuyncrwa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/grjyqrgiq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gwihgrsct.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gscekqhmb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/guesdzstq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/glcflekph.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gtscutsmu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gibhlohon.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gobeseekz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gejxvxbtz.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gcvenabzf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gbzovpgqa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/glneeaffd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gjxifkhwj.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gmgedjrlo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gbcxfxzgj.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gknpvtgtm.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gfctzvryo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/grmrwrcrk.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gaygowwoc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gmwaudmnt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gnggjefum.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gpbwfdyav.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gewrqwaho.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/ghntzdnyy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gubpujrer.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gpabxxioz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/geprpzyhn.sHtML


<!-- 参考信息 -->