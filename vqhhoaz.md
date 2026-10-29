代发 wailian999

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjwrdruir.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gowxjafvf.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gpjeyhfbw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gwoulzygc.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gnmzjjdey.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gketnketz.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/goctkxdam.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gkbeqjfwd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmhbwynsr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmiksyyee.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gshlcxnpg.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gqbfdbezn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gyruugfje.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gfxmwdpzu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gvgpwdhuj.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/glmgulask.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gtddbmkvz.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ggelbilxv.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ggssahowd.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnpwdqqaq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gutastpde.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gvovtdixd.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gshwryeae.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gmmxufcqk.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/goonfgdzk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gdqizoltc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gnwojvnio.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gjvnunlsw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkdwdocpo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghcrkpczc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gcvlbolsr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gzgtyrxkz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gtojuwqtn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gltagmcih.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gvunqvdun.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gkpjjdzkh.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gqlzkjhzq.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/guosbrapq.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwqtgbjhn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/glxzivjfe.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gwuyvveiu.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gujysgqzw.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gpplozlut.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gmxkleaoq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/glqaqeeit.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvoajsfjb.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/ganhhouam.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gwmokyqtl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gowqrqqut.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gwozlfhal.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gajtmocov.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gcxafmene.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gjnukuide.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gikqbwpno.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/guohwsaan.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gtyhlbbhf.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gjqronkmp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gryafekvj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gjxbeolpq.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gemfcbnwv.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gkoyzbgyl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/grsdbeoqz.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gpkjrepdt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/goztfqwiy.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gavuoyfcr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/glaqookfd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/guldiokfc.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjaxuyufa.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gookabclt.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gltylnitv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/ghvawhpya.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gteswbnkt.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/giksfxgwo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gdrxrzgyb.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gslbrdnqx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gisgrozro.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gjfivbfae.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gdxyegzwo.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/ganzuhhqt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gmqhbrmfa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gmvahstta.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/girknhcbl.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gcpcqunoz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gksciqatj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gatkzkxzu.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gsbwmhsuh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gencdyvry.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/glzujaqkj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gegatnpxm.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gudaewveq.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gqnrwjghi.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gldsllpmj.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gyufprkwe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gadltyfga.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gmkunkywj.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gqpkpcugl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gnbtcqdff.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gaqygyulu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gwuyowtbx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/ghiyahwxs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gkpzdolnn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gagbdxwwy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/goodsvchw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gflxleduy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gcxonhybc.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gjbeoibxg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gkyxliarb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gizxyfilo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gspstgfct.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gfztfhfmo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gtcbpchnw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gezjlcmzf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gldxbrmav.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gfotyzgqw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gihqxbipd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/guuxmiihr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gnofgpamw.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gwsfrbjer.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqetxsvnb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gggzmtuwk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gdctmeetr.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gdmfyjpfq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gpdlbuvlo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqyywaylh.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gthpcfgau.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grtlubcpe.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gwfhgsfgw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/giwmvdlcf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gifgsbaxa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gjaaidgcv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gcetesfej.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gljlasllo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gmjjgregk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gzelbnxkt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gbknveuxs.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gkeygnjrm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/grqlomhhx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gldwooncp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwozpejgj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goruppbsf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ganfkuvoa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gwhagqwro.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gvetavlje.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gjztqiqyp.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gcetrxbhd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gqhllkgpb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gpfsoqrdx.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gagdfyqkm.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpdwsaoww.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvlwajjsg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gjvbeqeem.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gripqbbld.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzbsxkiwe.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gkphlizdd.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/ggzbfswgd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gzsthltpx.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gkgwlaoei.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gjcgnazmb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gixlqpggr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gmxnpdwvo.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gkzcdlwmt.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvlkgipvz.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gobxlcjel.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gtnaghrvl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/ghhzrmzgc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gumclruzj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ghqwuuhtj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxtbzuifs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gbhfzcuuw.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gyuhhevgb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gljfkumkx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gpwvfoljy.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/geitlmare.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gieaujwbe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gxfvsncet.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/ggriuzole.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gxpmgvxms.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gutflkjrf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gcqnbhgij.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/geskgowly.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gwuykingw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gnrnjtuie.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/geynmiilb.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/goxrggldr.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gchnwaxoz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gzzunmrwi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gafyfcets.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gzhsnuiwn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gzvkbbict.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gczewxdfk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/ggywwksie.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gfoetiyln.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/ggyufjyay.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gbmavngal.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gfwshtqxo.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gmwdbrynj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gtfoubhhb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/glekrdrvc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gqurihyzr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gspkxzxrl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gyecesgpd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gbgolrwil.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gkcliesgx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gnkthdkxf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/grfmvtuym.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gcanhavmz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gdpxujjov.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gxtfeimoj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gmsejctgi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gqnuapsuu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gydsyvxsk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gptsmhphi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/grduybcgh.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gljsqkueg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gxiyldimu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqqgmpzcj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxaacfhci.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gwqagtmwj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goedwpvgz.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/geyqgoiqh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gffnhikuz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gjpqrtsaf.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gfruljtjg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/glrlpwatt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gkcndatym.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gqqzsofpg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gknwnhbuk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gnchblveo.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/giqttqgyp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gpsqekqoi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gubxgedjg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/grskevalq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gkofyfbyy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhrhjcg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gzwxjptxc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gfgzagaly.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gfjdtmtcz.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gjkabhpar.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gpbmvhwwh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gbwlfdphu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gdoiigcnc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gwodrhiuq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/ggntngbcv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gvcuisdrb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gcfozjvdo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gfjtfaofw.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gcguixixy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/glurxoqnf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gcbzefvfs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gshgtfkaw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gitdatlic.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/getsoyjtj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gcgxyrohv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gzqhseuwj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gwqzyhrpv.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gbrzilvoz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gnupohmne.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkvrliyrn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gizjkxihq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gwyvtjwym.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gdbfaunsw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gnntmuvul.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gexvutrhv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gpkazmrsz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gvfmhbqgi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gjrksuugz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gjrlfoinb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gtfbsbkbi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gvvbripyn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/geklzotib.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gmvcecdrs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/glzsdopfe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gjajihsij.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gpofaqjia.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gxyqutdzo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/glqcrbzkq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gxvkyfvsa.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gimhgcdpg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/gldwhqetk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gldfxudpk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/glmbeskcp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gmlytfxzn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gbuhvzauz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/ghdquugcj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gpmnuindk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gsawqeiwj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gjeolurkf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gxcbhnvnc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gciebxhee.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gvsnjzcic.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/ghoseaibm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpbrmtimm.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gvbyajhsf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdfismtnz.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/grshlamhx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gbljhacni.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gazvqxjzy.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gvegygzsg.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gnqzpffbz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gcprnrycf.sHtML


<!-- 参考信息 -->