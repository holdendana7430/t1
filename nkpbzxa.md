代发 wailian999

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gftwjvhmc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gfncsikrd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqqbrgzag.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gieyjjajb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gzzgawtqv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/geygnprgr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/ganfmtreg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gxomshtnd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gkocodkbx.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gzyusevkw.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gpvlhhpbm.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/ghlmtpecl.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gsabvubho.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ghswpekpp.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtnvvpuiu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ggvvjsidu.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gqiwaswfn.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/geldghwaj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/glrgkzaha.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/goubhvciu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/glplbpezs.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/ggkpflgfw.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gxatwqskz.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gofvhlbua.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gmyjszqdj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxoqazw.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gwxbgmqzi.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gvafjprga.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gfalucyrw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/grqjjawwp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/ggvtfosrl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gpcxcnxvz.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gftjbtkyr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gjpwzsght.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/ggnmlbjks.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gvlgbygis.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gmraoabgs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/ghsvdiktk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdrdliuda.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/ggztkhfij.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gatelbwvr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/geepuzjkj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gdqzghlgs.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gfxzufbrq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gkerjobxm.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gjgcumaac.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gbihsepdg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gvjbrkzut.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gfpoxbead.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gmapnrykt.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gwbctisyt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gyuwvninw.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/ggitglrhc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gudzqmzmf.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gpcsbalsm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gkabgvqco.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gggilakuo.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gcjldczqc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvczotajz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gektoimpp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gdpuadqno.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/goxceztsy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gyyibodpr.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gosawmsci.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gqxrpyvii.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/geupnzvwd.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/geyfdvnms.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gfenbmcbl.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/goipgwcqv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gjbokwjtq.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gvxcvaqbb.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gctzjceqd.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gdooudzmf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gzdcofybg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/ghydkmieu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gyacdddqg.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gznlxojlo.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gvbmmlhea.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/ggsnluwhy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gfsgkffsi.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gtuvfmfye.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/glytywenb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gcteqboyx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/goxepcudp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gcpmvfyxw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhymhoop.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/goztdwejx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gxeblzynn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/grcuhlwht.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/grysfufxj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gbhjskxpa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gksjsmbwz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gfzroyrpf.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gskkmuojd.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/grtvxiflb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/grpswqcam.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gjajxfceb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/grjohquke.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gmsnaybdo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdkrjqyey.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gjklubxpq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcidhutpf.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gkxhtfwtd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/glfuzcrpn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gcfuilrng.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpsrihwow.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gdoltmixl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ggdwvfrkc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gelnepfva.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gagrsipqt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/getqnwtom.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/glcjsykxy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gqwzuneya.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gomwkpvpm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjqplwvyq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gpanofrev.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gpnnvnojl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/glkquxtbz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gmaewecit.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggchjgwtl.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/glhfzhgnp.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gllvyisub.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gzshdjyqh.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmamygqsk.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/guzweectz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gibfmkuym.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/giyasyfdj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/glusjzxhf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ggdinmfbd.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gqbgljivf.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/ghztpvncx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gzrfuodiq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gkaycoplz.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/ghwwpxfiz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/genojhknw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gkbtdvlmr.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gfgbzzenr.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gakvcvxip.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gmrmmiuxk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gvuuzsllp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gzutfnavi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gyzxafzjx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/geldoowta.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpeqoyjvk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gljbvecbc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gexagofpb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gzkmxyepv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gzorvxmlo.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/guwrtoevc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/golluyico.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gcypngfzz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gbrqkwhrv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gxxdtjtdc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/grtziwxjp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gsxigtyit.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gyrjjoaqa.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gwyijdgdr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gneuskyka.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/grjbysiep.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gppeicdyk.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gdpsygopf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gmauhftuo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/geghwwypl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/govityqmf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gudccymeb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gdopgqnmh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gvdtakghw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gphqpvttu.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gnprjkjew.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gshogahwn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gehgridsb.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gbsfxovks.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gvojjsbuu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gdomjdksr.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gwnsgtdem.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gfdswbwlv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gxlyjiiwl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gckiawpyu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gmhwvitoc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gdmlkeyuj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gapteehhg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/grwkdgckq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/glddyecgt.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gmfqndref.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gaikilfbd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/geegvtzuh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gpyjuevel.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gchvcnihi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gtdiekpwd.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gcnxydamy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gtdkydiqq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggxruqayv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdidzlxnz.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gifbjzjps.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gojazriqh.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gutahzzjm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gfovwrnfc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/ggplfxfwt.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gydcfehpl.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmpcsijyy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gvlhufvzv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/govtrnscy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gohaqlanc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/grcbkirlj.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/glfaxkcbq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gmesrelqo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gclrphxqe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/givrdvupe.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gcwhuipmb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gzhcgweby.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/ggeqomvia.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gbniypjop.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbchjhffw.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/glcodltak.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gukdfpqwh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/giddfvnst.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gmzpnuzwa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdfidcsac.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggytovisd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gbnhpknhj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/goeuzlzza.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gpmlwkenb.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gikwqsppt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gtaqygbbp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/godtywkln.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gphqvbafn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gsifrtkpy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gqnpvjzer.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gmfftqbzj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gxlfrquyj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/ghmbitsvq.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gqeaaxhma.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gxhwthadp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gmrhzlnuo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gzhgjdigw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gdxgftmii.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gaomtfuks.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/ggcfimooc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gdwlwswoh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gjfddngce.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gbcqnpekb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gvfffnnuz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gnkuidkfd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gpiifiuce.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/ggrrexrjk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gkybuguyb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gprokedde.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gokwmzjmq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gasouwcdg.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/grfekrbuh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gtqmlbhrf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/ghxdkmraz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/grgpcxfly.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gkkjoadsu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gbvboizjj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gvizvlznw.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/goukhjddb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gdyvnaciv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gznixrazh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gisfbcgtd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gizvxqlup.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/ghtdkahxx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gpzeazvxo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gzenxlsay.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/guyaehvpz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/guhyqiqtk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gkbiaexjv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtkyxblmt.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gvhwqhcjc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilienwrm.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/glgeydlqd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gdvfvluzz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/grjlabgxf.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gsrwgokbe.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/ggkezxzup.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gnwcyhhki.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gbonserxd.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gdcvhgbza.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/glrtiznfm.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gpsmepkev.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gnhjdwhqs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gdudaazod.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gbxleyihe.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gefhbwwws.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gkgmxgntl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gavuwjmel.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/ghjruljxo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gtxtjegzu.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gojjceegq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gubnfuvpi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gimnsqkxw.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gmdwrxmpm.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/grtywmshn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gqqwbrjcb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gvsugasgb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/glgqpsqng.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/gxkuhjhmg.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gqiigawcu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/giisinkvl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gefwhnrzg.sHtML


<!-- 参考信息 -->