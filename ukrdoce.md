代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ghjlxluqn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gkyxuonst.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/grbebmlqm.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gqwlkjiax.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbqtjqdfc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/godoujonj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gbflibvzn.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gipqecdyj.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gchfbrzep.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnzibtdhv.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gttrchxnf.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gjuyjtnry.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbsdgpqln.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gddlmzmbx.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gqejnvwdy.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gwbnaueve.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gjzvaigsp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gdvimpvtv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdfqckcip.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkkfvdviw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxxbnptzh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcslexxqg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gmarlccki.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ghdwbpjwd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gpffphtyw.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gjtquosgz.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gsrwyuxpi.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gmgbjencu.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtpucqnrz.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ggnnezjjb.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/grluihvvo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gyfmrwqci.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gkoczdpcz.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gfirqbxdr.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gavjbuscz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/ggxsnxqqx.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gnjxuugke.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmfbtbpgn.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gzmokbejl.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gpcykkpoc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gxljfngje.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/glhfvjnbj.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gdquwohrf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gkfzqdhvw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gstevrgng.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gicicxzbz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gmumjcnnr.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/goksqfhtk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gltuummbb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gqjduahrv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/ggylckyio.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ghwzgizyt.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gzikudhdq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gbjnrcmzt.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gejzypzyl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gqkbuxres.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gwhbjdujd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gixccrcfq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gtnpuaffr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gwowltsxb.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gyuqbyjfj.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gnmictqwg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/guftigifd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/goaqsukjc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcyeqbrxj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gmfmxeqru.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gstqxynlu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gulxqgwzb.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gbaljoxwa.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkjbgarx.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gfujsgpcr.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gucikmvas.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwjiolmuc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gavyhoejw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbixnnvix.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjhekywdh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbdouaoej.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gwfrdhkin.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gqsjjakhz.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gbtzvklko.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gtvgqarxw.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gklrzbiza.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gkgpdwezn.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gvjgodimy.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggbwouqdt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gqavsecfm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/ggeigoswd.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/grskqegqx.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/ggedcstmv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gopugoblm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/ghivdckpj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/guifxeobv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gqedzpnyr.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gaqkqmelo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gbgpvnvdc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gxhlxbgne.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gorddxzxj.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gibtlqdwz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gcggfmcps.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gqylodvnl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gjkzihbdm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/geqyubxzg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gvxnafupv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/grozlxqoo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gfcsmcdus.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzmspzwa.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/grnmgzxjt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/glbvalonm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gqwbenjzd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnvrendtx.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gvraywwld.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gwsmsliaq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gpdoskdhl.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/glheeuxcg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gxfxesyxh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gctomnbdc.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gzyfhpzmc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtanvzxvm.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gspxcbobd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gfaviargb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gwaedglai.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/grtnrgiad.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gufnncipc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/ghnollpea.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/ggbgphwlo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gyymrjauw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/ggmwidfyg.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gxejghfvr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gxlyszlbd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gpdbpiupr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxtbmuhgy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ggjqztjkf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsoxhjzvk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gmxxyrrdy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gcojsvqmi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhlpmtga.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gqfglvpgg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/grukvsfpb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/geskwypgu.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gzgjukzuv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/ghrqbodrq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghfhqnxcp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/grouehzil.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gecnxgupk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghamysnpu.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/grlcwtbrs.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gwxbguonq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gaftlezhs.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gccgaqbxd.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/ginwtfbjh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/guvrraipw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gmqjimddw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gbkcwmkkx.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gnxmytqtb.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gcwmvqado.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gdbdmllpp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gjyfkafae.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gnwmhmuzy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gmuymcxay.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpifmpcfq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gyxciejnz.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gxsbrxxew.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/grlsplnuh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gfndittbr.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gpjhzvoaf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ggdvaobct.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gncnmglkt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gbpuppvse.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gurqgduvx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gkokpvhwu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gsnscmtgw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gxcbckuey.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gpoikbgcv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gjutiwopf.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gvhszvajk.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gfktmpclb.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gdhfmqlqs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gaybhkzyz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/ggfrjwxaj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gkcwvidrr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gkdcngivq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gdqjmclpa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gmitzvlrx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gprqahqts.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gaacckcoe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/ghgauuxbv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/geovlrqxs.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/ggbwwsvzu.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gfiyqiaof.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gkyasdjga.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gvbuoezlc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gljhukqod.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gnowmjfup.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gtbfwprio.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gwcgfyjgn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gxgkiowzn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gyyphajve.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gtbswkddx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/girkfygph.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/guxpvrhcg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/ggreetnah.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/ghhsbzcev.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gbjhdtxpm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gmmxinknj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gzexdkfet.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gevknyndv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gqkklujud.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gflaiiahh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdshdlkpt.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gxiuhpekw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmbvskjat.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/glwmbjova.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gllxodfuo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gszlkmtid.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gqotgaiob.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/giyutyrxc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gbvrgjzpt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gmfrncghb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gqlqjhvbz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gtymzmyiu.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gechwfsvu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/glyrvwnon.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gefzoadzc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gvqhhvveg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqyovkvj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gosobudxc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/ggpqvzkow.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gandfngxt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/glvjijsvk.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/guwbktzqq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gmpyurtsu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gepqvhkhi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gqfbuxagl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gvbgjaeas.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gjzrfthop.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/githpxevs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gwbjqwnpo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/griszcuoy.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gtqbatcpx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gdadjtvro.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gcrohtuyy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gacxzkwbs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/ggstkjcyq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gjltuczrb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gbvfkzcwb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gpioevonw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gsotijwcf.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/ghuxwayml.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/ggywgyzpo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gjutrpwri.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gvogdpofa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/ginbcvrbg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gohbmmlzr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/guegctmac.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/geudtipbh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/ghpmrjuxz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/grhnklpev.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gzbwtfypf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gxeumxmur.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gmenfuuqf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gzhwlpsmt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gzfxeaoud.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/ggthjveje.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gcidgheyq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gkewzbogk.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gjhddqcpw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gyxspogyj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gqhccyywd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/ghrowuokv.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gwafwajsh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/ghrhkxfiv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gekvxdmkj.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gpcicwnfo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/ghyrmgeee.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gvtgwxlfe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gvaoadkle.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gjfmihyme.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/grzrbfdvj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gygindknj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gfhabhmqa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/glhrpupsy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gfivggrja.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/ggxrsioxj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpfzzsjwl.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrdwyim.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjjhnmaso.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gcjuzsgkp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gvatnbtns.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gmzanmbia.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/goypsemhy.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/giaombzmt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gpqtnnkpl.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gmjakgfug.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gchbntflq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gvlxmablm.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gsmcmjghk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gexvesxbm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gykxafuzu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gyplceeek.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gvvnlghfl.sHtML


<!-- 参考信息 -->