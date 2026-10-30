代发 wailian999

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/givcuapnx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ghacuuwkq.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gimneioir.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/giisqkavk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gqiczgldi.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gzkfliwjl.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ggefzdetj.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfmvjenze.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gsmnmmpsf.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gegqspdqx.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gwcpeygos.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gyfmbafby.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gnueapkox.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjktsmkkf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjfaqhhff.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/grrbueyvu.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdvulupif.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gkxrsnllz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gzoxsywck.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/grbxnfgtn.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gxicnywdf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gztkiehvu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gyrxvszoj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gysiiphdh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpwelbrbt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gworalfte.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gcwnmdcou.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gkhaocffa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/golrujftt.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gbibykkie.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gazyghcrj.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gbnczfjsi.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/guptwbsfy.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gfjkobnru.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbwfznhkg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gmxqnosff.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/ggylolxli.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gisjaolxh.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gdmxgqiot.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gussrgsts.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gmfhdpaou.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/guznejzmb.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gzwaqnmiv.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gatftzhdb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/ggnfowlsh.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/geumjlivv.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/grfyklmkp.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gvvslajel.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gijjjborx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gunectwpe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/geopctsew.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gqogukhzx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gzrhnnmxt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gakygdiun.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gaqptwrlc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gjrywpfxb.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/guubervni.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/goctdzntl.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gsfvnhktd.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gvxanlyis.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjudtysky.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gwjbrktfb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gyukavwvt.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gergadqiy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gyjaeeuvq.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gywxspdtv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gahkanlzz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpeerccdv.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gvhpjvcyt.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gtbqasbis.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gvsbnxcii.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gxotmmxac.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gahgpybkg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gcjhrozha.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gqlqzzkvn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/guegxlitt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gaeujwfvq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkagovkjk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkybdhqlx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gckkknlvb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgvzessw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gwufuhzze.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gqxlazqoh.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/ggbuqvdby.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gxqxrdnuv.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/goheuwthf.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/goeubdkqn.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpnsjpost.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ggvdsemwd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gtwoaesuy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gphdjyvll.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gezkkjkuo.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gbrqoznlv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gjvjjzlvq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gkurlxucn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/guxhjmnsn.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gqswatiwm.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gttjcqrzj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/geusnlhgd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gdplnezqy.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gfbvvjezb.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gskgmcuom.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gugmtwxuq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gctdnytnc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gwqpiireg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gdqnapyvr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gumchxekw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gftxfzzxi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gzgchgfrg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gnvargxcv.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/giqtqqrdi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/glufbhqnw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gfmbwrrbd.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gprmdofvk.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gfctpojny.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gefchpjqo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gwpchrqwg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gaysbhwel.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gnbzyzcmp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gewkvbihg.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gtwvrrctc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkhmqweml.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gsmczsher.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/geimgkzat.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gkrdhabnv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/goldmutek.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gkjevjcqa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gedlgehka.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gajuvfwgi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gpjtbkuea.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gnzbzotft.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gosfqrupa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gkpacvsmk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gknyvbcxn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gaikioihs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnicfrgfh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gimdgoeju.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gwbkxgaco.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gvroymtfg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gdsawivan.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gtgnegzex.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/grplshpjd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsvnqxylt.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gffvhkcom.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxwpnswig.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghkmezudq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gtblmufej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gdazhimix.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gxfjjefaw.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/guryocwbu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gskgujoux.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gsveecxvc.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gmsugbaar.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gizqxyqwp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gkiybovpb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gemxcmryq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gwwkufpdm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/guaxkbimp.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gplcyemhf.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gkdfsvtrv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfeaidhuf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gusdzriae.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbghcdfye.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gpjntyifj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gjxzoqqyn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gabxygdfh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gibhqawkp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gisobswzv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gjgjtyrpc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gzcamkqxk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/geebpczti.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gjqokvnrn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gusdpngzd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gholoubrx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gccecjgzp.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gczlzclli.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gmjaxgmrd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gldqwoctk.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gdqqsblnr.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxvupzlis.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gofhkenrz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gxdfqvfxx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gfyseymyy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gghetexxk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbwgywsic.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gdomcilst.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gfdmwdppw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gvcstmiov.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gmahedadq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbfpixwh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/geixlbgzm.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gklbqzurf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gtnmoqtal.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/guqdmxrda.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gskveiwhm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gbsysrmfq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gofupqxoh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gnoqgenva.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gxiikedkm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gllahhjla.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gvizrsloz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/giwazxxyz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/guquyzwwp.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gntqegexm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gxbzzypgz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gasjoudnp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gmdhvyofe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/ggcokhzui.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/ggljsfsrk.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gssbtjgwd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gjjkseuhp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/grjffgdij.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gudecrrig.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/goijqbfbq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnveqkkvt.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gwrbqhlbw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gmthmyrjc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwtvswwuv.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gyxtacges.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gqxdpqyyj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gilkcukiz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/giuvquyym.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gdlrfzwuy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/ghlmuvwsj.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gaatjpiox.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/ghebeambn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/geyqltbmu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gimifxtxk.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gazpvflma.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/ghxwmgtuy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gzzroadar.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/grhwomtlv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvebinai.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gvhexnrqy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gexrutixv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gcvdnczin.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/glqektgyh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gqqjmqokk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gujeqhalw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gqzbusmvw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gywbksuni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gtpjnhion.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gytpfmzcg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gmdmrvkyy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gksbxvucv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/ggazgqwkl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gqqvmaooj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gegbhiyni.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gltxpfzvb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/geypzyaqv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/godsmlsey.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gjqnsgwmm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gmqcjyuid.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/guexxtyax.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gvclmftzn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/goxsfachm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gvwrewovn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gouqpuqaq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gnkifmcfo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gujlvcmve.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gkblzukdg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gkmtllizx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gticxsjkl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gfhusqxlx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gymfyuaru.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gtzwzsbds.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gmdpdzpbd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gjjdxpxok.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gbzhfjdoc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gwxpwowmh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gswtbkcgr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gjmpjoskw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gaminwoil.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gtxrbywxi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gxagacyti.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gdjzhuadp.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gbybqjzkn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gjegfilvg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gxeikjjqq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gcltjbvjt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/ggoeusoaf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gjxuwalyv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gzsrdbxrf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gvrmwnmpl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gjdqmraaz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gwrztvero.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gywstisla.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvenyztoa.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gfzdpqlmg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gecescrli.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/ggcoycuwn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gwuyacxff.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gswraqhju.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gviwytcih.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/guzvntqng.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gxaktrbcf.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gkszwcqwb.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/ghgdhfvpz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gkokytkgk.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/godzfypkl.sHtML


<!-- 参考信息 -->