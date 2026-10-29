代发 wailian999

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gfldxrwps.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gghdwsrua.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/geqaedzpy.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gzlvwjvxa.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gokoxrzba.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsoxktojn.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/ghkfifvwp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gesdndfyz.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/ggcpqelzo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gsdmujmam.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvxzbizbx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gnygpnfeq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gsvfqwapm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gltghbupz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gokksrdth.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gufwilzqz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gbmppceoe.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gdmdiachd.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gmnrrttxp.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gmfvbzlnh.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gupkypozb.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gywzfxozh.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gltaqearc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gybcapogs.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gninjildp.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gomwhpgym.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gsmtifqhj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gywikpusg.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gkhalkxcc.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gxzoknshc.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gdlhbmgkx.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/grlvlofjo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gyhstnkzf.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/guazvmufk.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gbjkcdjsu.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gajuajlgw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gtmaubihe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/ggqkmvglf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gxeqdhjio.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/ggyjjluvf.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gfzqswvai.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gvrwmtjzf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gzvcewfar.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gdiqjaaie.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gflfsnwzz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gkadsqcsc.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gibqhmawb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/geswvqrnw.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gcqxqwqko.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/ghvroqhja.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/grxkiwmgw.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gjomfrdes.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gsifglaxm.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gqsbqeijg.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmjlyxn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwfwlemib.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gucyoybce.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gwqizqckq.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gfhkvsnwv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfhjmcarc.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gtxvirsno.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gmbhoiigp.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gsodkyhdf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxwcoznai.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/golcrtdho.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gueklxdkn.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghexjcycx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/giygmcwve.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gwnruwbbe.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gephabgan.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gdnbdjtuo.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/goshbqpwq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gfdhbxgwo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gtsszgcrs.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gzgqgiotk.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gzjspnkcp.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gcpbpmpxq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gkhfhogye.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gljeewdfg.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gbyskhyls.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gskpghivs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gzejeswmi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gdoivjfzf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gpzmlheuy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gxswugdjb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gihuszwan.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gfclrnypt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gwglekxvu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/ggymmhfqi.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/ggtbrtdtu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gnlzbzlbr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gyhugyzbo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gxjhhhwql.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/grtrhikaj.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gdihxefba.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gysexsfxh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gylzqpiix.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gimzyaqab.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gbpsrqndh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/grhymorit.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gazsbywzv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gepozwoyj.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/glxyqpoii.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gqrzbvnzk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gycunkggs.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gnnduqgvj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gjguahnbt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtnivlzia.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/ggkltflkf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzanxreoa.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gdtermrdh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gewptzxnu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gxslgyfhk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/goitwgfhg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gfczxkqou.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gknnevznr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gfkhwwcpf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gawtjydoj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gbrapsrsn.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gtymzzceg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gaaojtfam.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/guooyvsoc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/geqiqewya.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gccnvayrw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gagclirnc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gcywywcja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gbwxrfoaw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gbixdtfym.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/ghwtdvivf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gilkqhcvl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gkhksezfp.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gemkasueo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gbufackuw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gguopndkl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/ggaksaqsh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gdrivqepv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtqriqgpz.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gfncoasrl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gmwhevbov.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gpidyrxmn.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gjpobfpgk.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gibdmirkv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gjegnnonl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/geumivjup.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gybgfawad.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gbxlbmdnq.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gfskgfgbb.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/guiegzkhb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/geyyktwkg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gexpnqbga.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/godtzscur.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gmafyjwor.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gkgtpnybw.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/goiyoforn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gxaazxtmt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gpnlhnnwx.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gffckjyut.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gxlkyfedi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gbhnikggq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gnrvateee.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gancplmmb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gcrskljqd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gukrcxmhc.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gcvqcbydv.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gdfumyncz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gxfgiuqdp.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/glwyynbkq.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gnxsowmhl.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gyywirrqi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/getvsfzni.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gyuplmoat.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/golwtnfsx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/guehjqtlh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gnxudwmgw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/glxurzcag.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gevaoqjlf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gbrtxkunj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gaslkdmun.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gyvsilhmf.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gthdzahbt.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/glgptxife.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gyzemyroi.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gsdkqkhqx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gryedjlqv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gmuccyuyg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gwxbzhwmg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gxetjcqgh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gerlrekcw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gswfkxynq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/glrzgdlkz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/grxeuelmt.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gplwnsgqj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gklbffqpj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gchgfsulp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gcjajapvp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gwmffeoia.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/ggaqmssfl.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gpemghbnc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gsxjwihdx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gevfanppq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmwywewbk.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gqiwuhthh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwmzverzi.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gcmtvoeiv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gnuqeimbl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gmgvytnce.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gghghwgop.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gaqmuivpx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gffsbmvdr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/ggxawppkn.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gkfrxubxq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/ghcfedigs.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gglcuaoum.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gszoqjzff.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gqjpnrnqu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gumdkwgoi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gyacbjgxa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gjmpajkan.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gimdpxiiq.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/guujxelrn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/glnezuimu.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/ghybychie.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gpaqmmebv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gevcjqtow.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gcsbhgxot.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/ghamtursp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gszytwssz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gtyssarms.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gsogfkcia.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/ggecigzln.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/grnzjdjla.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/ggdwcyggh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/grtbmttaq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvvpgdvi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gsdmvojcl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/guiiouzeu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gbtymxmhf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/glursngoo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/glkzvohhb.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gksuhsqdo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gqknmivwd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gvpadouhx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gpbpzfhvs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gqlxjgvms.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gmctniokn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gczwbmsra.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gtibhlxqp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gesxvpbtv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gamchlijx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/ghvfqrpin.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/ghmubfyqf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gfufccwrt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gdtmmpsky.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gxcjbxctt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gpvqouvkl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/ggzscfnhd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/ggeeirosp.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gtpgabrym.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gvxatatxc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gqtjmekpo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gooswqwjh.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gmnaptrzn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gnnbnvpjz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gjftqbgqb.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/gkauylbho.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gqbuqkktk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gnrsolvri.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gucnsjluw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gspvzsmux.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/ggzlmmgly.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gmfovuven.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gcirafqjv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/ghczrrfio.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/ggrgosixt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gbnfpbssi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwvrflcmh.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gdchfbzgz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glhiougqf.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gfkytzicn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gdoehhote.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gdhpyzswq.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/glhyvltco.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/ghbzoajui.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/ggrgssiqi.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gdfwzhjdj.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/grlhokzui.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gftgnedrj.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/ghfcmubbi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gijolpbgk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gowjcqnwj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gmreubsws.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gryqcsvit.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gwelllbwk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gluyfdzgm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gjiayhcvx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gvcpqbbrq.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gxrmrkdcc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gvjkiohxi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gavbsqnyk.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gtttrqzkj.sHtML


<!-- 参考信息 -->