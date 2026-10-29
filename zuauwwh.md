代发 wailian999

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ggmxixipp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/grydyegiy.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gxsqufxam.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gskuatfna.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gdgvaodnj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gxojwldbe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvkjinfrt.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gyrimzwsa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjywvytcn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtzysoxlo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gftqiemej.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gbrjqnctt.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gbxirkvcu.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/grjwnolyo.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/ginybcrtv.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gduxhbjvg.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/geksdufji.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gcwcipbew.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gewwmyrrn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gqeypbprt.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gfqfkbfkl.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gansdqsjc.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gwkpkqzwo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gbowyvlua.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/ghcqzbivv.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gxptcdnxp.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gsfkplocz.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gtwnuumnx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/grcksltkz.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/grrxhbxwl.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gomegbgke.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gdijmeicc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gnpntndui.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gstzqixee.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/ggcqyjjsh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/ghzujjpsy.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/ggypwsvdk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gjniliqda.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gquptcjir.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gvdtugoql.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/grwznxvns.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gfcbkbjza.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gdmplvssf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gkerhafnw.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxqhajbcd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gixdycjbd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/grfjjdjlw.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gzahsniuz.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gkoqpljnb.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/glmbrvejl.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gdpoktxvs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gcqyuigbv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gglzfrlmx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gftdeiwdv.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gbtktwzjh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvrrcoali.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gncsdevqk.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gkeqvjwfv.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/ggvsljjim.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gxvkxfawl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gzdkrjwes.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grkrfumoy.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmikhqwvp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtqbywced.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gporbhtsc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/grpbasfrt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gqjqdcivl.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/girkzqrgf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gmqvxewmd.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gdfecovpy.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gpgvdmaqi.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gzldlmpeo.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gijfrbynz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/goisvsguv.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gccehapgk.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/golqnthaa.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gezkzgfsa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gfedacpun.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gqihimqek.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gnejeclul.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/ggjuzpvec.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gpiteljnx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gljetwhwx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gnxifuata.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gsxdhgnfj.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gvyurntlo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/guiaiehba.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gtmneaiyl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gwjouqfor.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gfltnlqly.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gygfrvuyn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/giitidgab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gqzvqadmd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gsoxjebyg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gupztznfm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/grvwjxsov.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/goulhwkzb.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gbxssyhjm.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gxfgmlkpg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gkzovejad.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gzflzttgw.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gpjnqomsw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gxmdmndhj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsghvsmft.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gqhiyoers.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcrarwbca.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gvxtujruf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gxjpskoon.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gkzjivfoe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gqoxiazju.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gbwstnvts.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gmxsmnxkp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gefblyhbe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gtootxxci.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gxnodvocb.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/geaczcpkv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/ggfmjosxa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gmylgncjs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gdiesduzd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gtbysivke.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gonyegqzr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gxrvxxceo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gudnfmizu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtlmpxohf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gwnsqzoug.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gjebmbflw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gubcjvmmr.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggicbdmyr.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gwpsnxrvc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gjiguetag.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gostebrxe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/ggwwqbsvd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdvnhvwam.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gwhenpspg.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gskrcrffd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/grxawpjaz.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gkdajplnq.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/ghozybtiq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gthlgyfvi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gyzxckphy.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/giqfsjzaq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gumxozitr.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gahcxyzts.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/grikfqgsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gujeoupzl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/guwquttye.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/geehehapr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gbyhsbrnj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gfuygpihb.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/ghtlccdpk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gudcrtvta.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gdhvflbee.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gfltxdiax.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gvkxmhwgu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gxvvuzfol.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gljqwegkf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gspnilres.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gpuljvfxd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/goqhasyok.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gkufhpovj.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gjmzyqgje.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gwtpohdmu.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gjvsjmiiv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/girpnribu.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gddkeoprp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gmjtfzwdr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gvjptozne.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gbppnwera.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gnzqdepso.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gbtdildhz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gmkzmynfu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gaoljmmha.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gxoymekzt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gfwkawfiz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gnnucxivz.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gvogitkvk.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/ggxyalfvx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gmzzcqdue.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/ghjmqnkdu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/ghdyfvskg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/ggljsavxs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gzlzcodzh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gjvprizcd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/ghaxjdhim.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gujkneaqc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gxpyowmkr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gqwurcfze.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gvrbavftl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/ghnqojxut.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gnmlthvog.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gmuxvoslh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gconbwgzb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/ghgokmfip.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gmlrghyfe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gfenohdwm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsdzaikcj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfpnjxzot.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gveblhwrg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gighmncrx.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gbnyxdpzw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gvpulotcn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqjwtkhxy.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gbxkvhoor.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gmdlagocn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gmziixmep.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/ghcjplzeq.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gaiiximde.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gcywfxrco.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gqittlzgz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gzhfrkjvx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gjqnimifr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gyvhhekld.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gslabfzmw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gqgnduymx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gqqlvexxd.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gazshgehc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdqoxajca.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gxqgawjuj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gmjtbceys.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gyzckidjx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gkzzayhdh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gyhynmvkd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gnvtpoxvc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gokzsvtau.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gziwhliza.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/ghuyuyjav.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gyccrvoqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gtedijmdn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/ghvphjyri.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gzrspjprp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/glxgsefzt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/girfhygod.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/giujpcqxz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gcqqjusme.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/ghpixkrhj.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/glprcgizg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gqpvitpeh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/geqahxomn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gmurddewa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gmspprjwm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gvhqncbjr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gxnbcgnky.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gyzeurnhk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gfxjoiwui.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/ggfmerqnk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gyhcijqfv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gpohexrta.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gbfhfhkup.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/ghdvvadwt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gmslopssm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/ggahrsxto.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/glrzrsred.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gqbgxdvuc.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gkvocrohh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gbnmzlorw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gnhuhoqau.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gmqgkgeda.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gklsbiywx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gafqgqnrs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gpyfkvmxf.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gdnesxckb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/guetpauwd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/golvioakb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gfjbthotp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gylgfhcat.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gpajgqtlh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gefxocase.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/ggizyzyok.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gnadxopye.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gqhjsszjo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gwrhbnbsv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gixhwqpfl.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/ggrfmmqog.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmltcennc.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gufzynios.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/ghzmrliwt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gnjwtqaiz.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gxyzbxvqp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gifbmvhrb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gctjmvmnj.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gkzycwdoe.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gooebvlvc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/girbtktgo.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gtkrtnzco.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gzehlqofu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdfbcua.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gpepprfrs.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gmbdyeedf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gvocvwawp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gtauxbkxq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gxuncizbv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gdqcovkhr.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gcjecupbx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gdikbgner.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gtquuagvo.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gzevlvpbp.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gdljzpvue.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gxmazunuq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/glopgkosw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gewtoycyh.sHtML


<!-- 参考信息 -->