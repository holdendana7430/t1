代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/guhbnqnqt.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gohkpsvwi.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbayzwvyj.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gsgxmgwva.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gcqcnmfny.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ghbyirybx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdpgqotvv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ggzremtbx.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwoqsjolv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/govumjllr.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/glejbrnah.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gamwjttvv.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gythsxjtj.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gdllgmfcn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gcwxhlcgk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gebumawqr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/guxydkufb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbuemjsug.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gdxezlqqr.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gmuppclvb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ggwzvkbqj.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gdfoesvwz.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/guhabofbb.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnbpnizvg.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/galgzgrvy.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gbhgjenlx.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gaqikekpa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gypejffyw.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gnrysmuvy.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gqfjmdfcu.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gtvfyzgly.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/glxhpfpcd.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gshedrhpv.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gbgynbrqa.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gfksyoxdi.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gxzyibcra.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtkfzlupz.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gkwpkysfv.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gkrznnbcd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/ggpejbojb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/ggagptntv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gbnvfpttl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gsjcahtbg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gahhmnlqo.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gnyosscds.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/giqxftvdr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gmeesftkk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gmisltiht.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gpmerwjqt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gvnfshyjs.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gfomtapkg.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gngcdbbjp.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxxxnpvch.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gtyyyviso.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gcgphvyjq.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gcbhoscow.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gofgyvbce.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqrnojasu.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ggcxpsnew.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gvlvgisvg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gibiqcpak.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gxpqocopl.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gspilahnu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gmmwembhc.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gavsgffqq.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkjhaeey.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gyozgwpro.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gpyihngrl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gifozlmji.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtzbkludr.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gaaaktbge.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnnbcxljb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grjjkywgq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gutcaorfl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gydraedts.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gxsbitnar.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/ggvlxtmiv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsncbaakf.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghgvindan.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gmfwtaclj.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grsdhmtxl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gmdcpasrf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gobxfcydl.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gbcuxybhr.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gnfxwdcqo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gyoyvvsvg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/geaeuvbfs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gskakxonq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/grgpkrvlk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gtceqrflh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/goumvfyvy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gsxzmamvb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gxfscbnqx.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gjkdwkzcy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gquljlybg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gjyflxvfu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gtzpsschs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfsqvjhop.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gqalpecxk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gocorntdd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/givcluwjg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghsnerkoc.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gopshidbe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gowmrjnvi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/guudnzlzc.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gladcxuir.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gzywmqalk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gliywcnlt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gujbimwue.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/ggvoefklf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/grnauwpxe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfcfjfuzr.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gmkmwpmzi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwftsyzul.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gjykkkddi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gnucjgmrd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gghjekzxc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gzuyezmns.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gfnehlhbs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gxnkqyfmk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gbdbulfln.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gloogclii.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gypakdtxk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/guqacoxvj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gvuqjzjdk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtsfjrsyp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gnhvotgji.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glarzhwsm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gewixvyxi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/ggfjfuujq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/giijocvjr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggxzummab.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/glsiscawj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gwfuvuhrt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/geyixoohi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grsddjafc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ggxkvexij.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gktzgvacr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gikwvcxpb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gtikoixgs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/giknqinyh.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/ghdttkjmu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gfswxiuhn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gpdnjwoji.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gekaogjdo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gjqojbtkx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gmkoocmgq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gqbzgioye.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gwfooicap.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/glfsreteq.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gfyzeimse.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gwhnexnaa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gqtjdsnqf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gogagtklb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaqupybkg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gyojoorvf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gvkfqglnu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gwzkzxlco.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghsmteduc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gmwgdjcwb.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gbhvxhszb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gmkzvazlx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gyohdewvd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/givtqfmbm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gofiaykwx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gfzvprspd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gmyuypvna.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gqekohedp.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/ghilronby.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gnbwdlkry.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gqkauxykk.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/greaztfqe.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gttavgzor.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/giroyjrey.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/grjtukidx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/ghsuaeoqs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gywjfyiji.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gjupqsgxn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gryzoyval.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gbygoquum.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gijiddazf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gosjldmgn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gwcijiewk.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gclptulfe.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/giwgeuzhr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gjkyjlgod.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gzmwayttk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/glbumqjjq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gaqlkclez.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gwzkvldbq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gpvkkgbsj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gtcvupwrf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gwmxwgslf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gchsctgur.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gpqoulwqc.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gdgjfctpy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gknxyefby.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gwhllgveg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/glqzossuq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gsikmwohf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/grxfqixvd.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gtprekjzp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gettfmznz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjquevxrp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpwcbogou.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gtpxgkmdi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvjnkskuy.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gxrwdzebg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gpfuvldct.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwpvzpnus.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/ggtupktwl.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gcuyoghky.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gakjlfwxy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gsohqmrxc.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gxvdzemtd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gethanirw.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/grpcoiyku.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gqejwagoh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gdkwxkswp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/grmlntziz.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gikhvards.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gjmedlsmq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/grlnisgre.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gccglmwsq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gyezjthvr.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gsmnsgahr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gmszjafws.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gqdlssxxs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gpkxuaxah.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/ghwxcysbm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gvndkjeao.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gwjivgsfh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/glnhfzqvg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gahwyzrjf.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/ggisdjaxo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gbqnmjxfo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/guxxsvgyw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/guetvmfte.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gzdpnmaud.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gqgygwwjq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gezvuqomv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gucpwfnns.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gxakbmtmx.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gfcfeztck.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gvrnbvjmv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdrjobciy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gpbrxsrel.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwohdojcm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gzgkipmlc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gmrsxvgup.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gksfffceb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gumfdzeoa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gszrsbrjg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/girodrene.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gyjxbnfiu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gcmqiuwhz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/glvavmdfn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/ghrlqikqm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gnqiekopb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gpvwlsbar.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gedlbntxj.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/geklbcegp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gphzwlqvo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gjmijjnde.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/ggghurtlp.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gdkgctbyt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gufqnqsxj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gdypdatus.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gikupeuuc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/giqsvvlfg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/glywtdlxj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gpugwlqbg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gtsskhysz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gnsgxakhk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gatojafxr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gnyazqbdi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gfcnvowky.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gepnvwaqe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gbxffopye.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtfoyaqxw.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gwijuyfqb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfqfwoqth.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/gtfyebpdx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gouqiafen.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gtsrrcnfj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/giiblhzqh.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/ghznibiis.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gdgncyjeu.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gylqjzipa.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gxsplfbky.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gaaqonlxw.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gqlpblkwq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gadomiysd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gjxswiudf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gmgpdwvcd.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gcydmulhq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gsadomdki.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gkwhjvida.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gjrgeitce.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gtubacckl.sHtML


<!-- 参考信息 -->