代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gkzwsxnuu.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/ghrhyuelc.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/glnjnojre.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwkljri.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gvybufsgi.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gsqcwtlrd.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gwklgsjea.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gjghdgkuj.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gtkzgivgb.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gkgnhxljo.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gpgbyrhey.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/guesrwhpa.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gesoikrhv.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/guvhufkvb.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gpawkwblp.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gpbxlyxiv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gpvxuqbsc.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gtjcsttze.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gvkxnegnn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gzalgwzcf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gjzpptmls.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/glytvlmck.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/ggljtuzzu.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/ghfliellt.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gogclnnil.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/grwhhijhy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gdutismgd.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gtygjmgrn.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gkptipuye.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gchoexmwj.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/galjwodcu.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/ghdqbilqu.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gpoblvjqu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gbggpaibw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gibxhgrao.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gsnaaxwhq.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gyouwlchv.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/grnjkgvqm.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gfdkdlbie.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjvsflypi.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gogeucmfb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggtmmjggh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsokkyahn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/ghhofzbwj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gtasruzaw.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/glntwkcsk.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gauxskjha.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gzubrjpbr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gnhimiuvb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gscarvjqb.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcusrohbp.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gozanoqwk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gwuumkcaf.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gsgdmuxps.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gdhemoklr.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/glurstzia.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gdhcdzsmh.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvroqilkb.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjizzxlwp.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggcgblrgl.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gosztfhzf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gqpfenaya.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gvplzzlvz.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gaulcyjyb.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gobleadxk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/ghvchqjju.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/glcickktt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gkuojspdw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gablwipsw.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gmeemqcbu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gezvsfqvy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gzukasufp.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gsydaqggn.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gswdivnps.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gtcwprlfh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbqpsrptr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/goexvdtkh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvyowgwqp.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/ggjincdtd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gvytpfeky.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gksmockxd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gcjxxsnhc.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gxzxlzcyr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gbnvyfzfc.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gqemnohkl.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/geeiszozq.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gcvllramx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/goxquedvc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gjkrysnjh.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gpcksugsm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gtxsqjpvd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkfajyzou.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gxwdlefyd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjicpkllr.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gqwehggup.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gbgqdydzr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/goehgdbqo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gakfjvskw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gwotxmfqr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gplogpimv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gwljhrmle.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gixunjgqw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gcakylztk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gryzsdstk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gbvxjoxpv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gwsumfapb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gskpyntvm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsxkbtklr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gvtgdoudd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gmdrkpaff.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gwxnerjul.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/geyuslhsd.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gdsvpykaz.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gcspljmwi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gxramocjp.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqoctnpvf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gftklokfx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gpoeqqqyl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gtdrjyuli.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gowesswpg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtzmphsfo.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gjzqpigkf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gboymjjda.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ggjlfzzej.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gseexwxto.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/glrwvknwz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gzfnryvvd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gfelcckpn.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gqcofkwul.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gspwykzic.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gvyzgsztn.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gqqowkjxb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gwjkulztv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gnskxupth.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdttuwnsb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gwtziytgc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gsnstaigm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gqyxbvjkg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gbbcsvazr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gquunrnqa.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gkcysrzem.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gncohonwn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gjofnkoaq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/geipjnuog.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gknkdseuf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gmzfrooxj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gyusfiuik.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gchtrghjs.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gkxhnrcnt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gybtggljg.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gcexftkzp.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gmucmsfrx.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gsusyeiik.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gfzulrpgn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gpqmkrjxo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gztuhsfvh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gohqjhaez.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/grhmozhut.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gtkgwfbhy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gfvloxqtg.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gqxzhehgd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gyqrhvezj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gwqpuzuur.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/ghcgozdtk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/ggubhmaus.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gdqhwwkhm.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gglrvghzi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gcvfymkje.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gckdjsqdb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gfixcgcmj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gchxjksbi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/grotoagri.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/govxvncfv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gvgdkaild.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gubcjelet.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gwurzwuwd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gnnkdzsqu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gwpsvhgbg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/ghpqrwjiv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gykxvqaog.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gvflubwii.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gvkdcpjqj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gwnfzyugi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gezrayejc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpwsbxpmb.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gghoneork.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdvsjszyx.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gnrqvuqjz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/geeowkion.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gsivszwzx.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gntabznai.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/geogzuqyn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gqzuwqtoi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gwslmnqoh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gkwagttsh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gadpvhnug.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/ghccabhog.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gzvrhounw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gmpgacidc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gcyszskgb.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gsuofamme.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gknebejgd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gldvqyopw.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gdlcjtfkv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsugsqxiy.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/glrtoanps.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gpmwxtdke.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gaupkkdna.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gtkolornn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gunxdibes.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/ggxfowdre.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gtdqvicrx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gmbphtiil.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gecraxdor.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/geadhlpkk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gftmwzzno.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/guxdjcdtl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gkhpxxgbw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gjoesqedb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gjepyazuu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmvotyvr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gssjvsppb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/ghblqwlyj.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gxfcjkxro.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gwfgiffap.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gstymumnl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/ghdkyojjk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gcjkhfhgg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gmztpimcu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gdxbthmcn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmdzhrr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/glbdprsog.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gghcnolla.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gbyzzrawa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gyonliqed.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gnrmrqzdc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/grhyxfdgk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gytylpwvv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gxdsporha.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gqrfqycjc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gaqfvrvxy.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gxsoehhxp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/ggxcpoifx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gbmkdkyuc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gjahbrsye.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gauvwjfoy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gohszsaux.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/ghjnjlvyg.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gnqwpfaas.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gflbqurzk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gotdwcayc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/ggjemwtud.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gdwxwgskj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/guaofxdag.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gclmfoijs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/guifiqvro.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/girzobuib.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gcctjviem.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gnconbsvo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkqptzfjb.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/geqjerovz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmmrvprjk.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gjpfijnxf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gpxjcyuvu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gihbjoakl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/geabwrppo.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gblvzspxz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gqhsszdgt.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/ggwazezve.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gefblycwu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gnojfuaqf.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gniredqua.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gdhrzltpv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gwdhjcuen.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gsvnpimda.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gompdhbuz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/glvdkxlgl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gbjwqqcee.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gvjesijqy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gtaqnegyl.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gfwcnnfin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gtzrmvkdz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gefnpmgyi.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gufhkhpsg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gqxxwbtye.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/goxryehgh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/grnkjrqes.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gcbbxsqtx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gxtphkvxf.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gjtexqgqy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gbkhqxcrt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gtmznqzwl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gtomjtzea.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/giktliaxv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gdpcsebon.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gnicctwwt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gtgjpxbgn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gyavzlitw.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/glkpdpxik.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gmitvmfyl.sHtML


<!-- 参考信息 -->