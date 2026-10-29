代发 wailian999

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gevarwqam.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gnbwcyjub.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gtyiaanhq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gasbtzpww.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gazpqzopz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/geplyyigq.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/geokekknk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gciodvlub.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gbbnqdewg.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gnxlcadvq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpzkhtsio.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gfbvewhiu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gcfvecssv.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gftiihqee.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gkcenecxu.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/ghmhmulyh.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gyakfmfdk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqjikiwfr.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggxamifos.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/goodgjaku.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gjuhkqjwm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/grvcbngjm.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gfijlaxin.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gkdujhrnu.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnhxnjvta.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gksoeshjs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gsrjodjzy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gspuoikki.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/giqxzwkpm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/goeagbtzl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gygdwhpjs.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gffylwjyz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gtqhcniqv.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gmsxwzpdm.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gahhcumqh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gimtwcphc.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/godrpxkxd.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcdzcjqru.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gfsnskryz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gdcdtrbge.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gbsnmqmip.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gjpihakfu.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gywyycuks.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpwybokkh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkkcxqklq.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gzzvdtfkn.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gpbbvtmdk.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gqoddajqd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gfiflgsmt.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gzzkumbam.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gurbpjjrn.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gtjgtmvku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gkadvoosh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmxibvkx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gdqayrqlk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gmeyfgvsh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gualcaxnm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gxnwclfcs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gwwtvdifd.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/ggipqyrta.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ghaqsvyuy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/giodlbtdi.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdgvrrjoh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/ggxdvwgro.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gurepudbj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gtjjvkgqs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gsgirhrqp.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gljmeozfp.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gueokjdyd.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gmxcotzjg.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gvpmkmbdl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gxkwdxdrx.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gsqmgosoe.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/guivegigu.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvinvbpwk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gmcxatqdd.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gzmnxkfjp.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gyaykxlfv.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/glfvtpzsy.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gcmnpcoed.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/glashanvk.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gnyzumeeu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzjwydyxo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpitcqw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gghrrrhub.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/glwpvdlhb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtcrslaek.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gglmxkuog.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gfflleorf.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gaxznhggq.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbqweovzf.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gdhzhctys.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gyebckizj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gcyzxoxcj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gmqfisehv.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gtsqhweem.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gmdffupww.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gdkahfruc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gheupvisq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gjwqhqqsp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gsqcuhpwb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gegsjpdsi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/ghnftuarw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gxroegxho.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gcjckhtta.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gjivqbiep.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gyhtvkwjw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gfknrmeuq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gvddbpyfh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/grmmyyzis.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gyfsejyzq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gyoaqofxo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gidhpzbfy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gqhdyfbut.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/geqbcwxmh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gipswqvmm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gytpktshd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghxuuqblv.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghpliixbj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/getoelucr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/giuttkmnq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gkahthlam.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ghxrzsnzx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gixwsdkbu.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gokosrrdz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkvmigiet.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gofikhcqe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gbzlypsfv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdctxhlsg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gqijjfrat.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gmvpoqlbe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gmtwgnfdp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/geikxphvv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gakuluxno.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gglxnbrnv.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gfnckgdnu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gsdbjhvcv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghpyengxe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gthoxicwz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtxnjwmro.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gumeftwnl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gsakfyzas.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gnpclyjod.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/giidssrgi.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/giparstki.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/graybtnsh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/guprncarj.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gwcnhzjts.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/grbbolhpa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ggofuowlp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/graqyxajm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/guvhmqdvh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gknlqrpny.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gousconur.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gcfxcrdkz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gbroqowfg.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gociwmpsw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gttmagnmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gndkmtxll.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gitotgagg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gaqkikyas.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gptyrfsky.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/geufgnjwg.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gkvnhsqgi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gxirkkdif.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gwistwhfn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guldvffqs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gknjpnpoj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gqhiurqwl.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/glvzmusui.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gwykqzrwc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gspfwavcx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gyualgatr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/ggcxruncv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gdopzhhkk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gduxfxfwd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/guffuentn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gabzkhgzi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gagvkmsgk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gpajukicl.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gpwrmwpfc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gohawhjmr.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gigsyhekd.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gazexinxb.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/grlgdlqap.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gzzqssoiy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gtukumhhy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/ggignsogy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzujhemap.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gtqkasaqt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gnudcpfed.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gqybvtbuj.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gfqwvwibv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gcaqwxjht.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnmbwoja.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gqvtaliqo.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/goudivkvh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gvrjjyrpd.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/ggkylypdt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gobivewcx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/ggfkutwcd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gxikubbll.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gvxvbutye.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gewpgqglg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gyzlnbiit.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gmzepuhyg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gkqidyzyo.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gczcypkzs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gcibwqurn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gvofiadfk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gcgksslsn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gpgregwth.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gseaczjvq.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gjhupkkqm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/glpfzemiw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqsuavflj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gldvqrrtx.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gmxjgtxdu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gikcmefjz.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtocaihpi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gqfjndkve.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/glrytuner.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gxugzkalr.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/glrkrckuw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gaactlpve.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/golujtrop.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gtzjlponu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gcoopjszm.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gxjmlfotj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gseorjgla.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gpbvqeouu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gyqihffyo.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gbkdzhtie.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gspnrqime.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gawurztzc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gqdzuiqer.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gyuhhphpa.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gkuwnwjnx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gcswsorlc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/giherkluj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/ggfrbqalm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/goyiczcyz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/ghhkukkxp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gzzlnrwqc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gceyfmtoz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gjajqgfro.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gsjhitdly.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/geqviqihg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gvurattya.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdycamfby.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gtsznfnrs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/ggwcuduwy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/goiwscvbn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gtxfztypz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gjifshcub.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/glillbdlo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gmedfmoub.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gvilwimpq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gxtsrdycc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gbntbuusa.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gkiygowfm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gjflgwwcx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/glpmapess.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gunhpdmis.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/goowxapox.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gmblafsfp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gcrgbtfjt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gxgprkyig.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gdkbwgztb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gkwxmbexw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gwxbsazjz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gpkzkpiam.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gufggfhxa.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gkrrcqzkn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/grffrudij.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gcbtknyif.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gpkiqaqtu.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gajqvlcyj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gwodxaesi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gqlhyfadd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gnyofnqei.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gwwucgvqc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gicerrapm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gtlpzyjxa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/ghmfhaprn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gntnfbixy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ghqanrhrf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gltamkmkn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gzjfacunh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gwgdpbpwy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gbvristog.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsvmwyczr.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/gwzneevbo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxpzddozf.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gtmzkzokq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/goeyngoqr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gjstxizaq.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gvsjiqnmr.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gsdibyrvp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gneggzpjo.sHtML


<!-- 参考信息 -->